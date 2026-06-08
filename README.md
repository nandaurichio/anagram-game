<img width="1534" height="243" alt="anagram game banner" src="https://github.com/user-attachments/assets/b8a9b0e4-7495-4fbb-9329-785834cbdabf" />

# Anagram Game

Um jogo de anagramas desenvolvido em Python para terminal, inspirado na estética retrô dos sistemas MS-DOS.

O projeto foi criado durante minha participação no Code in Place 2026 com o objetivo de praticar lógica de programação, manipulação de strings, organização de código e experiência do usuário em aplicações de terminal.

## Objetivos do Projeto

* Praticar programação em Python
* Trabalhar com estruturas de dados
* Aplicar modularização e separação de responsabilidades
* Desenvolver lógica de validação e controle de fluxo
* Criar uma experiência de usuário simples e divertida no terminal

## Funcionalidades

* Seleção aleatória de palavras
* Embaralhamento dinâmico de caracteres
* Sistema de dicas
* Controle de tentativas
* Interface estilizada utilizando códigos ANSI
* Reinício de partidas sem reiniciar o programa

## Tecnologias Utilizadas

* Python
* Biblioteca padrão `random`
* Códigos ANSI para estilização visual

## Conceitos Praticados

### Estruturas de Dados

As palavras e dicas são armazenadas em um dicionário Python, permitindo separar o conteúdo da lógica do jogo e facilitando futuras expansões.

### Modularização

O projeto foi organizado em funções independentes responsáveis por tarefas específicas, como exibição da interface, embaralhamento das palavras e execução das rodadas.

### Tratamento de Entrada

O jogo realiza normalização das respostas do usuário utilizando métodos como `strip()` e `upper()`, tornando a experiência mais robusta e amigável.

### Controle de Fluxo

Loops, condicionais e validações controlam as rodadas, tentativas e reinicialização da aplicação.

## Como Executar

1. Certifique-se de possuir o Python instalado.
2. Clone este repositório.
3. Navegue até a pasta do projeto.
4. Execute:

```bash
python jogo.py
```

## Aprendizados

Este projeto permitiu aprofundar conhecimentos em lógica de programação, manipulação de dados, organização de código e desenvolvimento de aplicações executadas diretamente no terminal.

---

Desenvolvido por Fernanda Aurichio durante o Code in Place 2026.
