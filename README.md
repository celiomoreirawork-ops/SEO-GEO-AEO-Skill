# Auditoria SEO / GEO / AEO — Skill para Claude (Edição Brasil)

Versão em português do Brasil, adaptada à realidade do mercado brasileiro, da skill [SEO-GEO-AEO-Skill](https://github.com/SNLabat/SEO-GEO-AEO-Skill), de Alex Labat.

Audita automaticamente qualquer site nas três dimensões da visibilidade em buscas atual:

- **SEO** — Otimização para Mecanismos de Busca (Google e Bing): title tags, meta descriptions, estrutura de headings, schema markup, links internos e qualidade do conteúdo
- **GEO** — Otimização para Motores Generativos, as buscas com IA (ChatGPT, Gemini, Visões Gerais criadas por IA e Modo IA do Google, Perplexity, Copilot, Meta AI): sinais de E-E-A-T, clareza da entidade, densidade de fatos e autoridade dos autores
- **AEO** — Otimização para Motores de Resposta, para trechos em destaque, "As pessoas também perguntam" e busca por voz: schema de Perguntas Frequentes, headings em forma de pergunta e respostas diretas

---

## O que muda na Edição Brasil

Além da tradução completa, a skill foi ajustada para quem tem um site voltado ao público brasileiro:

- **Tudo em português:** conversa, relatório, status e glossário em pt-BR, com datas no formato DD/MM/AAAA e valores em R$
- **Relatório em papel A4**, padrão no Brasil (o original usava o formato Carta, dos EUA)
- **SEO local à brasileira:** Perfil da Empresa no Google, buscas "perto de mim", endereço com CEP e UF, telefone com DDD e botão de WhatsApp com contato também em texto rastreável
- **Sinais de confiança brasileiros:** CNPJ e razão social no rodapé, Política de Privacidade conforme a LGPD, reputação no Reclame Aqui, página de trocas e devoluções (CDC) e exigências do Decreto 7.962/2013 para e-commerce
- **E-E-A-T com registros profissionais:** verifica CRM, OAB, CRO, CRP, CRN, CRC, CREA e outros em sites de saúde, direito, finanças etc.
- **Idioma e domínio:** `lang="pt-BR"`, `hreflang`, `og:locale` `pt_BR`, uso de `.com.br` e URLs sem acentos
- **Schema com dados brasileiros:** `addressCountry: "BR"`, `priceCurrency: "BRL"`, telefone `+55`, CNPJ em `taxID`
- **Mobile em primeiro lugar**, considerando o perfil de acesso no Brasil (celular, 4G e franquia de dados)
- **Crawlers de IA no robots.txt:** verifica bloqueios a GPTBot, OAI-SearchBot, PerplexityBot, Google-Extended, ClaudeBot e outros
- **Expectativas realistas:** avisa que os resultados enriquecidos de FAQ e HowTo foram restringidos pelo Google em 2023 e que o schema Speakable só funciona em inglês, nos EUA
- **Ferramentas de referência** gratuitas e disponíveis em português (PageSpeed Insights, Search Console, Bing Webmaster Tools, Google Trends Brasil)
- **Caminhos de arquivo genéricos:** o original tinha caminhos fixos da sessão do autor, que não funcionavam em outras máquinas

---

## Como usar

Depois de instalada, basta enviar uma URL ao Claude e perguntar sobre o desempenho do site nas buscas:

> "Pode auditar o SEO do site minhaempresa.com.br?"
> "Analise meu site exemplo.com.br — por que ele não aparece no Google?"
> "Meu site está preparado para buscas com IA? exemplo.com.br"
> "Faça uma auditoria completa de SEO, GEO e AEO do meu site"
> "Quero aparecer nas respostas do ChatGPT. O que falta no meu site?"

O Claude vai perguntar se você prefere uma **Auditoria Rápida** (principais problemas e notas) ou uma **Auditoria Completa** (análise detalhada). Em seguida, ele rastreia várias páginas do site e entrega um relatório estruturado, com um documento Word e um PDF para download.

---

## Instalação

### No app do Claude (desktop ou web)

A skill é distribuída como um arquivo ZIP.

1. Baixe o ZIP deste repositório (no GitHub, clique em **Code → Download ZIP**)
2. Abra o app do Claude no computador ou o site claude.ai
3. Acesse **Personalizar** (Customize)
4. Vá em **Skills** e clique no ícone **+**
5. Envie o ZIP — a skill será instalada automaticamente

Não é preciso descompactar. Depois de instalada, a skill fica ativa nas suas conversas.

### No Claude Code

Copie a pasta do repositório para o diretório de skills do Claude Code:

```bash
git clone https://github.com/celiomoreirawork-ops/SEO-GEO-AEO-Skill.git ~/.claude/skills/seo-geo-aeo-br
```

No Windows, o diretório é `%USERPROFILE%\.claude\skills\seo-geo-aeo-br`.

> **Dica:** se você também tiver a versão original (em inglês) instalada, remova-a para evitar que as duas sejam acionadas pelo mesmo pedido.

---

## Estrutura do repositório

```
SEO-GEO-AEO-Skill/
├── SKILL.md             ← Instruções da auditoria (fonte da verdade)
└── README.md
```

---

## Histórico de versões

**1.1.0-br** — Edição Brasil
- Tradução completa para o português do Brasil (skill, relatório e README)
- Adaptações ao mercado brasileiro: SEO local, WhatsApp, CNPJ, LGPD, Reclame Aqui, registros profissionais e schema com dados do Brasil
- Relatório em A4, com datas e números no formato brasileiro
- Verificação de crawlers de IA no robots.txt e notas sobre o estado atual dos resultados enriquecidos de FAQ, HowTo e Speakable
- Caminhos de saída genéricos, que funcionam em qualquer ambiente

**1.0.0** — Lançamento inicial (Alex Labat)
- Modos de Auditoria Rápida e Completa
- Rastreamento de várias páginas do site (até 7 páginas na Rápida, sem limite na Completa)
- Notas de SEO, GEO e AEO com matriz de recomendações prioritárias
- Relatório de auditoria para download em Word (.docx) e PDF

---

## Créditos

Skill original criada por **Alex Labat** — [SNLabat/SEO-GEO-AEO-Skill](https://github.com/SNLabat/SEO-GEO-AEO-Skill).
Edição Brasil por **Célio Moreira**.
