# Politica de Seguranca

## Reportando vulnerabilidades

Se voce encontrar uma vulnerabilidade de seguranca, **nao abra uma issue publica**.

Envie um email para o time com:

1. Descricao da vulnerabilidade
2. Passos para reproduzir
3. Impacto potencial
4. Sugestao de correcao (se tiver)

## Praticas de seguranca

### Codigo

- Zero Trust entre servicos internos
- Sandbox de execucao com limites formais
- Prompt hardening contra injection
- Validacao de formato em todos os inputs
- Classificacao de dados e limites de output

### Infraestrutura

- 100% Cloudflare Workers (sem servidores para gerenciar)
- Secrets via `wrangler secret put`, nunca em config
- Service bindings via RPC, nao HTTP
- mTLS entre servicos (planejado)

### Dados

- Isolamento por tenant (namespace D1)
- Valores monetarios em centavos (sem float)
- PII nunca em logs de telemetria
- Zero cross-tenant access

## Superficies de ataque conhecidas

| Superficie | Defesa |
|------------|--------|
| Prompt Injection | Prompt hardening, validacao de formato, output parsing |
| Supply Chain (Tools) | Tool signing, version pinning, behavior monitoring |
| Data Exfiltration | Classificacao de dados, limites de output, egress filtering |
| Replay Attacks | Idempotency keys, nonces, request expiration |
| Memory Poisoning | Trust scoring, write validation, forbidden patterns |
| Noisy Neighbor | Sandbox de execucao, budget por tenant, rate limiting |
