# Contribuindo para e-artesan

## Como contribuir

1. Leia o [pack cultural](./time/CULTURA.md) antes de tudo
2. Abra uma issue no Linear descrevendo o que quer fazer
3. Crie um branch a partir de `main`
4. Siga as convencoes do repo (ver CLAUDE.md no repo de apps)
5. Abra um PR com descricao clara

## Convencoes

### Idioma

- Codigo, documentacao, issues e PRs em **portugues (pt-BR)**
- Termos tecnicos consagrados podem ficar em ingles: *middleware*, *pipeline*, *webhook*, *handler*
- **Somente caracteres ANSI** em identificadores de codigo (sem acentos em nomes de arquivos, funcoes, variaveis)

### Commits

- Conventional Commits em portugues
- Escopo: `gepetto/...`, `sitia/...`, `time/...`, ou `org`
- Nunca commitar secrets ou `.env`

### Codigo

- TypeScript strict — sem `any`
- Toda logica de negocio DEVE ter testes
- Valores monetarios em centavos (`number`, nunca `float`)
- Result pattern para erros tipados

### Testes

- Vitest + `@cloudflare/vitest-pool-workers`
- Nomes descrevem comportamento, nao implementacao
- Dados reais do dominio (mensagens de produtores, nao "test123")
- Rodar `pnpm test` antes de commitar

## Duvidas?

Abra uma issue ou fale com o time no Linear.
