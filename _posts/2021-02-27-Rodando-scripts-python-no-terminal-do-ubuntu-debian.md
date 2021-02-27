---
layout: post
title:  "Rodando Scripts Python no Terminal do Ubuntu ou Debian"
description: Seja Bem vindo ao 8Bits\Code, Boa Leitura.
tags: python pip ubuntu debian
---

O Python é uma linguagem de programação muito famosa e por isso muito utilizada em diversas áreas da tecnologia, desde desenvolvimento web até em Inteligencia Artificial.
Hoje vamos aprender como roda scripts python no terminal do Ubuntu ou no Debian e seus derivados.

## Crie uma pasta teste
Para fica mais organizado, vamos vriar uma pasta para o nosso projeto teste, para isso digite o seguinte comando em seu terminal.

```
>> mkdir teste
```
com isso você terá uma nova pasta como o nome de teste.

## Acesse a pasta
agora vamos acessar essa pasta, para isso digite o seguinte comando:
```
>> cd teste
```
## Crie um arquivo de texto python
Assim que você precionar ENTER voçê irá para dentro da pasta, agora podemos criar o nosso script teste, existe varias formas de criar um arquivo de texto, nesse caso vou utilizar o nvim, fique avontade para criar com o editor de texto da sua preferência.
```
>> nvim main.py
ou
>> vim main.py
ou
>> vi main.py  
```
Ao apertar ENTER, voçê vai ter acesso ao arquivo, precione "I" no seu teclado para poder editar o arquivo.

## Escreva seu código Python
agora com o arquivo python aberto, vamos escrever um código para podemos execula-lo no terminal, para esse exemplo, vamos fazer algum bem simples, vamos escrever um "Hello World".

```python
print("Hello World!!!")
#=> prints "Hello World!!!".
```
Após ter digitado o código, agora você pode salvar e sair do editor, para faça o seguinte:
1. Aperte no ESC do teclado
2. Aperte SHIFT  :
3. Aperte ENTER

## Execulte seu script no terminal
Agora voçê está com um script pronto para ser execultado no terninal, para execultar o script, faça o seguinte:

```
>> python3 main.py
```
se tudo deu certo, voçê terá como resposta um "Hello World".

## Execultando o script com uma virtualenv
caso você saiba o que é uma virtualenv, fizemos um post explicando como instalar o programa que cria virtuaienv, acesse ele Aqui<a href="https://8bits-code.github.io/2021/02/17/Criando-Uma-Virtualenv-no-Ubuntu.html" target="_blank">Aqui</a>

caso já tenha instalado, digite o seguinte comando no terminal:
```
>> virtualenv venv
```
Voçê pode mudar o nome "venv" para um de sua escolha, após isso, vamos ativar a sua virtualenv, faça o seguinte em seu terminal:
```
>> source venv/bin/activate
```
Aperte enter e terá sua virtualenv ativada e pronta para uso

agora vamos roda o script python nela, para isso digite o seguinte comando:
```
>> python main.py
```
novamente você terá o seu script execultado.

## Criando um executável python
Para criar um executável python voçê tem que escrever uma código na sua primeira linha do seu script, para isso abra o seu script com o editor de sua preferência e digite o seguinte código na primeira linha do mesmo:
```
>> #!/usr/bin/env python3
```
salve a modificação e digite o seguinte comando no terminal:
```
>> chmod +x main.py
``` 

agora vamos roda o executável no terminal, para isso faça:
```
>> ./main.py
```
como das outras vezes seu script irá roda


## Assista a explicação completa no nosso canal no YouTube

<div class="embad">

<iframe width="100%" height="400" src="https://www.youtube.com/embed/CGf-l0ElRFM" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</div>


Esperamos tê-lo(a) ajudado(a) a sanar suas dúvidas.
Até o próximo post...
