# Bússola Brasil 2026

Ferramenta cívica e não-partidária que compara suas respostas a um questionário sobre temas do país com as posições reais de candidatos às eleições gerais de outubro de 2026, para todos os 26 estados + Distrito Federal.

O usuário escolhe seu estado, responde 25 afirmações (escala discordo totalmente → concordo totalmente) e vê, para Presidente, Governador, Senador, Deputado Federal e Deputado Estadual/Distrital, quais candidatos mais se aproximam das suas próprias posições.

**Demo ao vivo:** _(adicione aqui o link do GitHub Pages depois de publicar — normalmente `https://SEU-USUARIO.github.io/bussola-brasil-2026/`)_

## O que este projeto é — e o que não é

- É um projeto pessoal, independente e sem fins lucrativos, sem vínculo com nenhum candidato, partido, coligação ou empresa.
- Não é um produto oficial do TSE, não é uma pesquisa eleitoral registrada e não recomenda voto em ninguém.
- Todo o processamento acontece no navegador do usuário: nenhuma resposta do questionário é enviada a qualquer servidor.
- Todas as posições atribuídas a candidatos vêm de fontes públicas (planos de governo oficiais, votos nominais, declarações e reportagens), sempre com a fonte indicada. Quando não há fonte confiável para uma posição, o tema simplesmente fica sem dado para aquele candidato — o site nunca inventa posição.

## Estrutura

Este repositório é intencionalmente simples: um único arquivo HTML autocontido, sem dependências de build.

```
.
├── index.html   # site completo (HTML + CSS + JS + dados dos candidatos, tudo embutido)
├── LICENSE
└── README.md
```

Rodar localmente é só abrir o `index.html` em qualquer navegador — não precisa de servidor, Node, nem instalação de nada.

## Publicando no GitHub Pages

1. Suba este repositório para o GitHub (veja instruções de deploy que acompanham este pacote).
2. No repositório, vá em **Settings → Pages**.
3. Em "Build and deployment", escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`.
4. Salve. Em alguns minutos o site estará em `https://SEU-USUARIO.github.io/bussola-brasil-2026/`.

## Metodologia (resumo)

- 25 afirmações cobrindo economia, segurança, saúde, educação, meio ambiente, costumes, diversidade, trabalho, instituições e política externa.
- Compatibilidade = concordância média apenas nos temas em que o candidato tem posição com fonte verificável; temas sem dado não contam a favor nem contra.
- Governador e Senador têm pesquisa completa de posições nos 27 estados. Deputado Federal e Estadual têm cadastro de nomes direto da API oficial do TSE, mas em vários estados é uma amostra parcial — isso é rotulado honestamente no próprio site.
- Um pequeno grupo de 10 afirmações mais específicas (facções como organizações terroristas, arcabouço fiscal, exploração de petróleo, demarcação de terras indígenas, maioridade penal, PEC da Blindagem, responsabilização de redes sociais, regulação de IA, tributação de apostas online, homeschooling) tem posições preenchidas a partir de conhecimento político geral já consolidado sobre figuras de alto perfil nacional, sem pesquisa nova nesta rodada — e isso aparece identificado na fonte de cada posição dessa rodada.

A metodologia completa e as limitações conhecidas estão descritas dentro do próprio site, na seção "Metodologia".

## Correções e contato

Encontrou um erro, uma posição desatualizada, ou é candidato/assessoria e quer solicitar uma correção? Abra uma [issue neste repositório](../../issues) ou entre em contato pelo e-mail indicado no rodapé do site.

## Licença

O código deste projeto está sob a licença MIT (veja `LICENSE`). Os dados sobre candidatos e posições são baseados em fontes públicas e podem mudar até a data da eleição — sempre confira as fontes oficiais (TSE, DivulgaCandContas) antes de tomar qualquer decisão de voto.
