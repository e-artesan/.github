# Gap Analysis: Alinhar GTM e Produto com a Visao de Data Moat

**Data:** Marco 2026
**Objetivo:** Identificar o que precisa mudar nos documentos e no produto para vincular a visao "financeiro -> tecnico -> data platform" ao que estamos construindo.

---

## Resumo

A visao para investidores e: "Sitia captura o unico dataset de decisoes financeiras e tecnicas do pequeno produtor rural." **Desde marco 2026, o produto implementa essa visao desde o D0:** 7 intents (incluindo `registrar_manejo`), dual-tagging (transacoes carregam `dominio_manejo` + `especie_alvo`), tabelas `rebanho` e `eventos_manejo`, cross-insights (custo/animal, mortalidade, receita/animal), contabilidade com partidas dobradas, contas a pagar/receber, audio/voz via Whisper com vocabulario agro, e infraestrutura agnostica em `@e-artesan/shared`.

---

## 1. DELEGACAO.md (Roadmap de Produto)

### Estado atual
- Fases 1-3 (75 dias): 100% financeiro (raio-X, engine contabil, DRE, balanco)
- Fase 4: WhatsApp avancado (audio, imagem) + escala NE
- Fase 5: RAG + memoria + evals
- Fase 6: Producao + seguranca
- Fase 7: Arquitetura multi-tenant

### Gap — FECHADO (marco 2026)

~~Assistencia tecnica nao aparece em nenhuma fase.~~

**Status:** Manejo implementado desde D0 com 7 intents, incluindo `registrar_manejo`. Dual-tagging em transacoes (`dominio_manejo` + `especie_alvo`). Tabelas `rebanho` (inventario vivo) e `eventos_manejo` (nascimentos, mortes, vacinacoes). Cross-insights no handler `pedir-insight` (custo/animal, taxa mortalidade, receita/animal). Nao e mais "Fase 3.5" — e produto desde a primeira mensagem.

---

## 2. README.md (Org)

### Estado atual
```
Sitia - Conselheira de gestao financeira rural
Visao: Gestao financeira -> contabilidade rural ->
       infraestrutura de decisao rural do Brasil
```

### Gap
- "Infraestrutura de decisao" e vago — nao comunica o data moat
- Nao menciona assistencia tecnica como expansao
- Nao diferencia mensagem para produtor vs investidor

### Alteracao necessaria

Mudar a visao para:
```
Visao: Gestao financeira -> assistencia tecnica ->
       camada de dados proprietarios do pequeno produtor rural
```

Ou, mais conciso:
```
Visao: Capturar o unico dataset de decisoes financeiras e tecnicas
       do pequeno produtor rural, comecando pela gestao financeira
       conversacional via WhatsApp.
```

---

## 3. profile/README.md (Pagina publica da org)

### Estado atual
Focado em "gestao financeira conversacional"

### Gap
Mesmo do README.md. Se investidores visitarem o GitHub, so veem "gestao financeira."

### Alteracao necessaria
Adicionar uma linha sobre a visao:
```
Primeiro mercado: Cariri, PB
Visao: O dataset proprietario de decisoes do pequeno produtor rural.
```

---

## 4. KPIs (29-kpis-metricas-roadmap.md)

### Estado atual
Ja inclui metricas de data moat (Fase 2+):
- Data Points Capturados (1M-10M)
- Receita B2B Data Platform
- Judgment Layer / Knowledge Depth Score
- Switching Terror Score

### Gap
- As metricas de dados sao genericas ("data points")
- Nao diferenciam dados financeiros vs dados tecnicos
- Nao medem a evolucao do moat por tipo de dado

### Alteracao necessaria

Adicionar sub-metricas de tipo de dado:

```
Data Points por Tipo:
| Tipo              | Fase 1  | Fase 2   | Fase 3   |
|-------------------|---------|----------|----------|
| Financeiros       | 50k     | 500k     | 3M       |
| Tecnicos          | 0       | 200k     | 2M       |
| Cruzados (fin+tec)| 0       | 100k     | 1M       |
| Contextuais       | 10k     | 200k     | 1M       |
```

Isso permite comunicar ao investidor: "em 12 meses, teremos X dados financeiros E Y dados tecnicos cruzados — dataset que nao existe em nenhum outro lugar."

---

## 5. Produto (Sitia features)

### Estado atual (DELEGACAO.md Fases 1-3)
- Onboarding conversacional (raio-X do sitio)
- Registro de transacoes financeiras
- Engine contabil (partidas dobradas, DRE, balanco, fluxo de caixa)
- Adaptadores regionais (caprinos, queijo, Cariri, seca)
- Registro de producao e eventos de animais (Fase 3, basico)

### Gap — FECHADO (marco 2026)

~~Registro de eventos de animais e tratado como feature financeira, nao como captura de dado tecnico.~~
~~Nao ha intencao explicita de cruzar dados financeiros com dados tecnicos.~~

**Status:** Registro de manejo e intent propria (`registrar_manejo`), nao feature financeira. Dual-tagging em transacoes cruza financeiro + manejo automaticamente. Cross-insights implementados no handler `pedir-insight`. O cruzamento e intencional e central ao produto desde D0.

---

## 6. North Star (00-north-star.md)

### Estado atual
Esta no historico/ como documento arquivado. Descreve o "Grafo de Conhecimento Unificado" com 3 saberes (ancestral, tempo real, cientifico).

### Gap
A visao do North Star e mais ampla que o one-pager para investidor, mas o conceito central e o mesmo. O problema e que esta arquivado — nao e referenciado nos docs atuais.

### Alteracao necessaria
Nao reativar o North Star inteiro (e verbose demais). Mas extrair o conceito core e integrar no README da org:

> A Sitia captura dados que ninguem mais tem: decisoes financeiras e tecnicas do pequeno produtor, com contexto (por que, quando, resultado). Comecamos pela gestao financeira porque gera valor imediato. Evoluimos para assistencia tecnica porque os dados financeiros revelam padroes tecnicos. O dataset integrado e o moat.

---

## 7. One-Pager anterior (00-one-pager-vc.md)

### Estado atual
No historico/. Focado em "Unified Data Graph" + MCP + zero-party data.

### Alteracao necessaria
Substituir pelo novo one-pager-investidor.md (ja criado). O anterior fica como historico.

---

## Resumo de Acoes

### Concluido
- [x] Criar one-pager para investidor com visao financeiro + tecnico + data platform
- [x] Adicionar manejo ao produto (implementado desde D0 — 7 intents, dual-tagging, rebanho, eventos, cross-insights)
- [x] Documentar captura passiva de dados tecnicos (cruzamento e automatico via dual-tagging)
- [x] Audio/voz via Whisper com vocabulario agro

### Pendente
- [ ] Atualizar README.md da org com a visao expandida
- [ ] Atualizar profile/README.md com a visao expandida
- [ ] Adicionar sub-metricas de tipo de dado ao KPIs
- [ ] Referenciar one-pager-investidor.md nos docs principais

### Nao fazer (por enquanto)
- Nao reativar o North Star inteiro
- Nao mudar pricing
- Nao mudar o GTM de 90 dias (50 pagantes no Cariri)

---

**Principio:** A visao e o produto estao alinhados. O produto ja faz gestao completa (financeiro + manejo cruzados) desde D0. A visao para investidor reflete a realidade do que esta construido.
