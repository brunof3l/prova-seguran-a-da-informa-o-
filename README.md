# Hub Interativo de Revisao de Seguranca da Informacao

Single Page Application em HTML, CSS e JavaScript puro para revisao de conteudos de Seguranca da Informacao com foco em estudo, memorizacao e simulacao.

## Visao Geral

O projeto foi construido como um hub de estudos em modo noturno, com layout responsivo e abordagem visual voltada para EdTech. A aplicacao reune:

- Modulo 1: Criptografia
- Modulo 2: Autenticacao
- Conceitos avancados com foco em Lamport, X.509, PAM, LDAP, RADIUS, OAuth e SAML
- Flashcards interativos com animacao de flip
- Simulado dinamico com correcao imediata e painel de explicacao

## Tecnologias

- HTML5
- CSS3
- JavaScript Vanilla

## Estrutura

- `index.html`: aplicacao completa em arquivo unico, com estilos e scripts embutidos
- `README.md`: documentacao principal do projeto

## Funcionalidades

- Interface dark mode moderna com detalhes visuais inspirados em ciberseguranca
- Navegacao por secoes com menu fixo
- Cards teoricos e visuais para revisao rapida
- Acordeoes "Visao do Professor" com resposta tecnica de prova
- Flashcards de memorizacao
- Simulado dinamico com:
  - 20 perguntas por ciclo
  - embaralhamento com Fisher-Yates
  - correcao imediata
  - explicacao apos resposta
  - tela final com pontuacao
  - botao para refazer o simulado

## Como Executar

Como o projeto e estatico, basta abrir o arquivo `index.html` no navegador.

Opcionalmente, pode publicar em qualquer hospedagem estatica, como:

- GitHub Pages
- Netlify
- Vercel

## Banco de Questoes

O simulado dinamico possui uma variavel chamada `bancoDeQuestoes` no proprio `index.html`.

Ela usa objetos com a seguinte estrutura:

```js
{
  pergunta: "Enunciado da pergunta",
  alternativas: [
    "Alternativa A",
    "Alternativa B",
    "Alternativa C",
    "Alternativa D"
  ],
  respostaCorreta: 2,
  explicacao: "Explicacao tecnica da resposta"
}
```

Existe no codigo um bloco comentado com a indicacao:

```js
// COLE O SEU BANCO DE QUESTOES AQUI
```

Use esse ponto para expandir o array com novas perguntas.

## Objetivo

Servir como material de apoio para estudo, revisao de prova e treino rapido de conceitos essenciais de Seguranca da Informacao.
