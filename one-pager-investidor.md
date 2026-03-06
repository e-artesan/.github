# Sitia — a conselheira do pequeno produtor no WhatsApp

**Construindo a plataforma e a camada de dados para o agro, conversa por conversa.**

**One-Pager | Pre-Seed | Marco 2026**

---

## O Problema

Um produtor do Cariri, na Paraiba, cria 50 cabras. Fatura 3 mil por mes. Nao sabe se ta lucrando ou perdendo dinheiro. Compra racao sem saber o custo por animal. Perde cabrito sem saber a taxa de mortalidade. Vende queijo sem saber a margem real. Nao e porque nao quer saber — e porque nenhuma ferramenta foi feita pra ele.

Ele nao usa app. Nao usa planilha. Usa WhatsApp.

Sao 3,9 milhoes de propriedades familiares no Brasil — 77% de todos os estabelecimentos rurais. Geram 10 milhoes de empregos, movimentam 23% do valor bruto da producao agropecuaria, e se fossem um pais seriam o 8o maior produtor de alimentos do mundo. Mas 80% nao recebem nenhuma assistencia tecnica. No Nordeste, esse numero chega a 93%.

Essas propriedades tomam milhares de decisoes financeiras e tecnicas por ano — e nenhuma dessas decisoes existe como dado em lugar nenhum.

---

## A Sitia

A Sitia e a conselheira do pequeno produtor pelo WhatsApp. Gestao completa — financeiro e manejo cruzados — desde a primeira mensagem.

O produtor manda "comprei racao R$850 pras cabras" e a Sitia entende que isso e um gasto financeiro E um dado de manejo ao mesmo tempo. Registra a despesa com partidas dobradas, classifica o dominio de manejo e a especie alvo. Tudo numa mensagem.

O produtor manda "nasceram 3 cabritos" e o rebanho se atualiza sozinho — de 50 para 53. O custo por animal recalcula automaticamente.

O produtor manda um audio dizendo "vacinei as cabras hoje, gastei quarenta e cinco reais no vermifugo" e a Sitia transcreve, entende o vocabulario do campo, registra a despesa em saude animal e o evento de vacinacao.

Quando pergunta "como tao as coisas", recebe: quanto entrou, quanto saiu, quanto custa cada cabeca, qual a taxa de mortalidade, e onde ta o desperdicio.

**Ninguem no mercado junta dado financeiro com dado de manejo pra pequeno produtor. A Sitia faz isso desde a primeira mensagem.** E cada conversa alimenta a camada de dados mais rica para agro brasileiro — dados que simplesmente nao existem hoje.

---

## O Mercado

| Sinal | Dado | Fonte |
|-------|------|-------|
| Propriedades familiares no Brasil | **3,9M** (77% do total de 5,1M) | IBGE Censo Agro 2017 / Anuario Agro Familiar 2024 |
| Sem assistencia tecnica (Nordeste) | **93%** | IBGE Censo Agro 2017 |
| Sem assistencia tecnica (Brasil) | **80%** | IBGE Censo Agro 2017 |
| Com internet (rural Brasil) | **85%** dos domicilios | IBGE PNAD TIC 2024 |
| Usando WhatsApp pra negocios | **96%** dos produtores conectados | ABMRA 9a Pesquisa 2025 |
| Rebanho caprino no Nordeste | **13,3M cabecas** (96,3% do nacional) | IBGE PPM 2024 |
| Rebanho ovino no Nordeste | **16,1M cabecas** (73,5% do nacional) | IBGE PPM 2024 |
| Agtechs servindo o Nordeste | **5,9%** das 1.972 do Brasil | Radar Agtech 2024 |
| Agtechs pra caprinos/ovinos no Brasil inteiro | **2-3** | Pesquisa primaria 2026 |

**O gap:** O Nordeste tem 47% dos pequenos produtores do Brasil e 96% dos caprinos. Mas so 5,9% das agtechs. Sao 8x menos agtechs por produtor que a media nacional. E zero delas usa WhatsApp + IA como interface.

| Mercado | Propriedades | TAM estimado |
|---------|-------------|--------------|
| Brasil | 5,1M | R$ 2B |
| LATAM | 15M | $4B USD |
| EUA | 1,7M | $2B USD |
| **Total** | **~22M** | **~$8B USD** |

---

## Como Funciona

O produtor ve uma conselheira no WhatsApp. Nos vemos um motor de captura de dados construindo um ativo que fica mais valioso a cada conversa.

```
CAMADA 1 — CAPTURA (o que o produtor ve)
  WhatsApp -> gestao financeira + manejo conversacional
  Texto ou audio: registra transacao, atualiza rebanho, gera insight cruzado
  Zero curva de aprendizado. Zero CAC. Consentimento total.

CAMADA 2 — DADOS PROPRIETARIOS (o moat real)
  Zero-party data: decisoes + contexto + resultado
  Financeiro + manejo cruzados, por propriedade, ao longo do tempo
  Dataset que nao existe em nenhum outro lugar

CAMADA 3 — PLATAFORMA (onde esta o dinheiro)
  Agentes verticais de IA raciocinando sobre dados exclusivos
  Credit scoring rural, seguro, extensao digital, cadeia de suprimentos
  Exposto via MCP (Model Context Protocol)
```

Pra o produtor, so a Camada 1 existe.
Pra investidores, a Camada 1 e o mecanismo de captura.

---

## O Cruzamento: Isso Ja Funciona

A Sitia nao trata financeiro e manejo como modulos separados. Sao lentes sobre os mesmos dados. Cada mensagem alimenta as duas ao mesmo tempo.

```
Produtor diz: "Comprei vermifugo R$45 pras cabras"
  -> Sitia registra: despesa R$45 em saude animal (dado financeiro)
  -> Sitia registra: dominio saude, especie caprinos (dado de manejo)
  -> Sitia responde: "R$45 em saude. Com 50 cabecas, R$0,90/animal."

Produtor diz: "Nasceram 3 cabritos"
  -> Sitia registra: evento nascimento, caprinos, +3 (dado de manejo)
  -> Sitia atualiza: rebanho 50 -> 53
  -> Sitia responde: "Rebanho agora: 53. Com R$800/mes em racao, R$15/animal."

Produtor pergunta: "Como tao as coisas?"
  -> Sitia cruza financeiro + manejo:
     DINHEIRO: entrou R$3.200, saiu R$2.100, sobrou R$1.100
     REBANHO: 53 caprinos, +3 nascimentos, custo/animal R$40
     ATENCAO: gasto com saude subiu 40% vs mes passado
```

**Isso ja funciona. Nao e roadmap. E produto.**

O dado exclusivo: "Esse produtor gastou R$X em racao E tem Y animais E produziu Z litros." Ninguem mais tem isso.

---

## Flywheel de Dados

Cada fase gera dados que destravam a proxima.

| Fase | O que captura | Profundidade do moat | Monetizacao |
|------|--------------|---------------------|-------------|
| Financeiro + Manejo (implementado) | Custos, receita, rebanho, eventos, cruzamentos | Forte | Assinaturas R$49-169/mes |
| + Assistencia tecnica (12mo) | Decisoes de saude, nutricao, reproducao | Muito forte | + ATER digital, contratos gov |
| + Decisoes integradas (24mo+) | Financeiro x Tecnico x Resultado x Contexto | Irreplicavel | + Credit scoring, seguro, supply chain via MCP |

> **Financeiro sozinho = util. Financeiro + manejo cruzados = exclusivo. Financeiro + manejo + resultado ao longo do tempo = irreplicavel.**

---

## Por Que Agora

| Tendencia | Impacto |
|-----------|---------|
| 85% de internet rural (era 35% em 2016) | Barreira de conectividade praticamente eliminada |
| 96% dos produtores usam WhatsApp pra negocios | O canal ja esta no bolso. Adocao feita |
| Rebanho caprino em recorde historico (13,3M, +3,1% em 2024) | Mercado crescendo, sem nenhuma ferramenta |
| IA generativa viabiliza interface conversacional | Custo de servir o pequeno caiu 100x |
| MCP virando padrao | Timing perfeito pra expor dados via protocolo aberto |
| Ninguem e dono desses dados | Quem chegar primeiro captura o mercado |

---

## Go-to-Market

**Dominar o Brasil primeiro. 5,1M propriedades — maior mercado, sem razao pra sair cedo.**

```
2026        Validacao (Cariri-PB)         150-350 usuarios
2027-2028   Dominar Nordeste              5.000-15.000 usuarios
2029-2030   Dominar Brasil                50.000-150.000 usuarios
2031+       LATAM (apos >50k BR)          +20.000-100.000 usuarios
```

**Meta Fase 1 (90 dias):** 50 produtores pagantes no Cariri, PB — com o produto completo (financeiro + manejo + audio), nao um MVP parcial.
**Ponto de entrada:** Caprinocultores, bovinocultores de leite, produtores de queijo artesanal
**Canal:** Grupos WhatsApp (500+ produtores ja mapeados), cooperativas, SEBRAE

---

## Modelo de Receita

### B2C: Assinaturas (Fase 1-2)

| Plano | Preco | Publico |
|-------|-------|---------|
| Chacara | R$ 49,90/mes | Pequeno produtor, gestao basica |
| Sitio | R$ 89,90/mes | Produtor medio, insights completos |
| Fazenda | R$ 169,90/mes | Propriedade maior, multi-usuario |

### B2B: Plataforma de Dados (Fase 2-3)

| Cliente | O que recebe | Valor |
|---------|-------------|-------|
| Fintechs | Credit scoring rural contextualizado | R$ 50-100k/ano |
| Seguradoras | Dados de risco com contexto de decisao | R$ 100-500k/ano |
| Governo (ATER) | Extensao digital + dados reais de campo | R$ 1-5M/contrato |
| Agtechs | MCP servers pra seus agentes | R$ 10-50k/ano |

### Evolucao de Receita

| Fase | Periodo | ARR Base | ARR Otimista |
|------|---------|----------|-------------|
| 1: Validacao | 6 meses | R$ 90k | R$ 150k |
| 2: Dominar NE | 2 anos | R$ 3M | R$ 6M |
| 3: Dominar Brasil | 4 anos | R$ 30M | R$ 60M |

---

## Vantagem Competitiva

1. **Dados zero-party como moat** — Produtores compartilham dados voluntariamente em conversas diarias. Nao e scraping, nao e inferencia. Compliance total, qualidade maxima. Cada conversa aprofunda o moat.

2. **IA vertical, nao horizontal** — Nossos agentes raciocinam sobre dados financeiros + manejo + contexto que nenhuma IA generica consegue acessar. A diferenca entre "perguntar ao ChatGPT sobre cabras" e "a Sitia conhece AS SUAS cabras, OS SEUS custos, A SUA regiao."

3. **Gestao completa desde o dia 0** — Financeiro e manejo cruzados em cada mensagem. Nao sao dois modulos. E um produto que entende os dois ao mesmo tempo. O cruzamento gera insights que ninguem mais pode oferecer.

4. **Audio/voz via Whisper** — Essencial para 63,6% dos produtores com dificuldade de escrita. O produtor manda audio, a Sitia entende o vocabulario do campo.

5. **Flywheel de dados composto** — Financeiro + manejo destrava integrado. Cada camada torna a anterior mais valiosa e mais dificil de replicar.

6. **Infraestrutura agnostica** — A plataforma Gepetto e o pacote @e-artesan/shared (audio, classificacao, sessoes, DB) sao agnositcos de vertical. Verticais futuras reutilizam a infraestrutura sem reescrever.

7. **Distribuicao comunitaria** — Guilda com 6 construtores. 500+ produtores em grupos WhatsApp mapeados. Crescimento organico via confianca, nao via ads.

8. **Track record do fundador** — Operando wattdata.ai ($1M ARR nos EUA) com o mesmo playbook de data licensing. 4 anos na TIKI (comercializacao de dados). Nao e a primeira vez em dados.

9. **Arquitetura MCP-nativa** — Construido sobre o Gepetto (nossa plataforma de agentes IA serverless no Cloudflare Workers). Dados expostos via MCP desde o dia 1.

---

## Equipe

**e-artesan: Guilda de artesaos de software. 6 pessoas, todas com equity.**

| Papel | Foco |
|-------|------|
| **Ricardo** (Fundador/CEO) | AI/ML + Produto + UX. wattdata.ai ($1M ARR), TIKI (4 anos) |
| **Miro** | Fullstack + infraestrutura MCP |
| **Mariana** | Engenharia de Dados |
| **Juan** | Marca + Comunicacao Institucional |
| **Hanna** | Operacoes (CL/CI/CD framework) |
| **Jonas** | Aprendiz (testes, dados, codigo) |

**Modelo:** Part-time, sem salarios ano 1, equity significativo. Salarios quando MRR > R$30k.

---

## O Pedido

| Rodada | Gatilho | Valor | Uso |
|--------|---------|-------|-----|
| **Pre-seed** | Agora | R$ 100-300k | MVP + primeiros 50 pagantes |
| **Seed** | 250 usuarios, R$12,5k MRR | R$ 500k-1M | Crescimento + modulo assistencia tecnica |
| **Series A** | 2.000 usuarios, R$1,2M ARR | R$ 3-5M | Escala nacional + data platform v1 |

---

## Por Que a Gente Ganha

Um produtor do Cariri cria 50 cabras. Nao sabe se ta lucrando ou perdendo. Ninguem fez uma ferramenta pra ele — porque ninguem achou que valia a pena. Nos achamos. E ja construimos.

A Sitia e a unica plataforma que cruza dado financeiro com dado de manejo pra pequeno produtor, pelo WhatsApp, desde a primeira mensagem. Contabilidade real com partidas dobradas. Rebanho vivo com nascimentos, mortes, vacinacoes. Custo por animal. Taxa de mortalidade. DRE, balanco, fluxo de caixa. Audio que entende o vocabulario do campo. 133 testes automatizados passando.

Isso nao e um pitch deck. E um produto funcionando.

- **Sao 3,9 milhoes de pequenos produtores no Brasil.** O canal ja ta no bolso deles.
- Cada mensagem vira dado financeiro E dado de manejo — ao mesmo tempo
- Essa camada de dados cruzados para o agro **nao existe em lugar nenhum**
- **$8B TAM** entre Brasil, LATAM e EUA

> **"Subir agentes e a parte facil agora. A diferenciacao ta em quais dados eles conseguem raciocinar."**
> — Jared Parker, CEO Watt Data

A Sitia so precisa de uma mensagem pra comecar.

---

**Contato:** Ricardo Goncalves | [email] | [phone]

---

## Fontes

Todas as afirmacoes deste documento sao respaldadas por fontes primarias. Arquivo completo de evidencias: `evidencias-mercado.md`

| Afirmacao | Fonte | Ano |
|-----------|-------|-----|
| 5,1M estabelecimentos rurais no Brasil | IBGE Censo Agropecuario | 2017 |
| 3,9M agricultura familiar (77% do total) | IBGE Censo Agropecuario / Anuario Agro Familiar | 2017 / 2024 |
| 8a maior producao de alimentos do mundo | Anuario Estatistico Agro Familiar (CONTAG/DIEESE) | 2024 |
| 93% sem assistencia tecnica (NE) | IBGE Censo Agropecuario | 2017 |
| 80% sem assistencia tecnica (Brasil) | IBGE Censo Agropecuario | 2017 |
| 85% internet em domicilios rurais | IBGE PNAD Continua TIC | 2024 |
| 96% dos produtores conectados usam WhatsApp | ABMRA 9a Pesquisa | 2025 |
| 1.972 agtechs no Brasil | Radar Agtech (Embrapa + SP Ventures) | 2024 |
| 5,9% das agtechs no Nordeste | Radar Agtech | 2024 |
| 47% dos pequenos produtores no Nordeste | IPEA / IBGE | 2021 |
| 13,3M caprinos (96,3% no NE), recorde historico | IBGE PPM | 2024 |
| 21,9M ovinos (73,5% no NE) | IBGE PPM | 2024 |
| 15-40% mortalidade de cordeiros | UFG / MilkPoint | 2023 |
| NE recebe apenas 14,1% do credito Pronaf | IPEA | 2022 |
| Pronaf 2025/26: R$78,2B alocados | Plano Safra / AgFunder | 2025 |
| <10% da producao com seguro, potencial US$28B | Picsel / mercado segurador | 2024 |
| Agrifoodtech BR: funding +32% Q1 2025 | AgFunder News | 2025 |

**Nota sobre o Censo Agro:** O Censo Agropecuario 2017 e a fonte mais recente para dados estruturais de estabelecimentos e ATER. O proximo Censo esta planejado para 2026 (IBGE). Dados de rebanho sao atualizados anualmente pela PPM (Pesquisa Pecuaria Municipal).
