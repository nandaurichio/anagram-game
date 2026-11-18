<img width="1534" height="243" alt="anagram game banner" src="https://github.com/user-attachments/assets/b8a9b0e4-7495-4fbb-9329-785834cbdabf" />

# Anagram Game

Um jogo de anagramas desenvolvido em Python para terminal, inspirado na estética retrô dos sistemas MS-DOS. A interface do jogo é em inglês.

O projeto foi criado durante minha participação no Code in Place 2026 com o objetivo de praticar lógica de programação, manipulação de strings, organização de código e experiência do usuário em aplicações de terminal.

## Objetivos do Projeto

* Praticar programação em Python
* Trabalhar com estruturas de dados
* Aplicar modularização e separação de responsabilidades
* Desenvolver lógica de validação e controle de fluxo
* Criar uma experiência de usuário simples e divertida no terminal

## Como funciona

A cada rodada o jogo sorteia uma palavra, embaralha as letras e mostra uma dica. Você tem 3 tentativas para descobrir a palavra.

```text
[INFO] Current Task: Unscramble the code.
-------------------------------------------------------
CLUE: The versatile programming language you are mastering.
WORD: YTHNOP
-------------------------------------------------------
ENTER_GUESS (3 left) >
```

## Funcionalidades

* Seleção aleatória entre 46 palavras, organizadas em 7 categorias
* Embaralhamento dinâmico das letras, garantindo que o resultado nunca seja igual à palavra original
* Palavras com espaço (como `VAN GOGH`) mantêm o espaço no lugar, então o jogador vê onde a palavra se divide
* Uma dica exibida em cada rodada
* Controle de tentativas (3 por rodada)
* Interface estilizada utilizando códigos ANSI
* Reinício de partidas sem reiniciar o programa

## Tecnologias Utilizadas

* Python 3
* Biblioteca padrão `random`
* Códigos ANSI para estilização visual

## Conceitos Praticados

### Estruturas de Dados

As palavras e dicas são armazenadas em um dicionário Python (`dados.py`), separado da lógica do jogo, o que facilita adicionar novas palavras.

### Modularização

O projeto foi organizado em funções independentes responsáveis por tarefas específicas, como exibição da interface, embaralhamento das palavras e execução das rodadas.

### Tratamento de Entrada

O jogo normaliza as respostas do usuário com `strip()` e `upper()`, então `python`, `Python` e ` PYTHON ` são aceitos da mesma forma.

### Controle de Fluxo

Loops, condicionais e validações controlam as rodadas, as tentativas e a reinicialização do jogo.

## Como Executar

1. Certifique-se de ter o Python 3 instalado.
2. Clone este repositório e entre na pasta do projeto.
3. Execute:

```bash
python jogo.py
```

As cores usam códigos ANSI e funcionam em terminais modernos (Linux, macOS e Windows Terminal). Em terminais muito antigos do Windows, podem aparecer símbolos no lugar das cores.

## Aprendizados

Este projeto me permitiu praticar a separação entre dados e lógica, o uso de dicionários e o controle de fluxo com loops. Dois detalhes de lógica ficaram no embaralhamento: ele pode, por acaso, devolver a própria palavra, então a função repete o sorteio até o resultado ser diferente; e palavras com espaço, como `VAN GOGH`, precisam ter o espaço preservado para o jogo continuar legível.

---

Desenvolvido por Fernanda Aurichio durante o Code in Place 2026.
