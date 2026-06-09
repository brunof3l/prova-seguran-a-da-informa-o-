# Hub Interativo de Revisao por Materias

Projeto estatico em HTML, CSS e JavaScript puro que organiza materiais de estudo em paginas separadas por disciplina, com uma home central para escolher qual conteudo revisar.

## Visao Geral

O projeto foi construido como um hub de estudos em modo noturno, com layout responsivo e abordagem visual voltada para EdTech. Atualmente, a aplicacao reune:

- Home com menu para escolha de materias
- Pagina de Seguranca da Informacao
- Pagina de Estruturas de Dados e POO com Python
- Dois espacos reservados para materias futuras

## Tecnologias

- HTML5
- CSS3
- JavaScript Vanilla

## Estrutura

- `index.html`: menu principal para selecao de materias
- `poo-python.html`: trilha de Estruturas de Dados e POO com Python
- `seguranca-informacao.html`: trilha de Seguranca da Informacao
- `README.md`: documentacao principal do projeto

## Funcionalidades

- Home de navegacao entre materias prontas e futuras
- Interface dark mode moderna em todas as paginas
- Pagina de POO com:
  - modulos de estruturas de dados, introducao a POO e pilares avancados
  - acordeoes "Visao do Professor"
  - flashcards de memorizacao
  - simulado dinamico com:
  - 20 perguntas por ciclo
  - embaralhamento com Fisher-Yates
  - correcao imediata
  - explicacao apos resposta
  - tela final com pontuacao
  - botao para refazer o simulado
- classificacao das questoes por tema e nivel
- resumo final por tema e distribuicao por nivel no resultado do simulado
- Pagina de Seguranca da Informacao com cards, comparativos, acordeoes e flashcards

## Como Executar

Como o projeto e estatico, basta abrir o arquivo `index.html` no navegador e escolher a materia desejada.

Opcionalmente, pode publicar em qualquer hospedagem estatica, como:

- GitHub Pages
- Netlify
- Vercel

## Banco de Questoes

O simulado dinamico atualmente esta na pagina `poo-python.html`.

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

Servir como base para um hub expansivel de revisao, permitindo estudar diferentes materias em paginas separadas, mantendo consistencia visual e espaco para crescimento futuro.
