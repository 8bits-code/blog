---
layout: post
title:  "Python - Criando uma virtualenv no Ubuntu/Debian"
description: Seja Bem vindo ao 8Bits\Code, Boa Leitura.
tags: python virtualenv pip
---

Hoje vamos aprender como criar, ativar e remover uma Virtualenv para gerenciamento de projetos em Python

Para que possamos dá inicio ao processo de criação é necessário ter o gerenciador de pacotes do pithon instalado em seu sistema operracional.
para verificar, rode o seguinte comando em seu termial:

```
// se ouver uma saída positiva mostrando endereço de algum diretório
// isso significa que o pip está instalado

>> pip --version

//caso ocorra algum erro, tente:

>> pip3 --version

```
se nenhuma dessas duas opções funcionarem, você deve instalar o pip em seu Sistema Operacional
para isso, rode o seguinte comando:

## Instalar o pip para o Python 2

```
>> python2 --version

```
```
>> sudo apt install python-pip

```
verificar se foi realmente instalado
```
>> pip --version

```
a saida do comando assim será algo parecido com esse:
```
>> pip 20.2.4 from /home/atrya/.local/lib/python2.7/site-packages/pip (python 2.7)

```

## Instalar o pip para o Python 3

```
>> python3 --version

```
```
>>  sudo apt install python3-pip

```
verificar se foi realmente instalado
```
>> pip3 --version

```
a saida do comando assim será algo parecido com esse:
```
>> pip 21.0.1 from /home/atrya/.local/lib/python3.8/site-packages/pip (python 3.8)

```

# Instalando  Virtualenv o Sistema Operacional usando o pip

Tendo verificado se o pip está instalado em seu Sistema Operacional, agora podemos continuar, a primeira coisa que devemos fazer para podemos criar uma virtualenv no Ubuntu é instalar a virtualenv, esse programa irá ser responsável por criar as "virtuais envs".

para temos acesso as funcionalidades, devemos instala-la utilizando o gerencioador de arquivos que instalamos na etapa anterior, para isso digite o seguinte código em seu terminal:

## Instalar virtualenv para o Python 2

rode o seguinte código em seu terminal
```
>> pip install virtualenv

```
Para verificar se a instalação ocorreu de forma correta, digite o seguinte comando no seu 
terminal:

```
>> virtualenv --version

 //  terá como saída no terminal a seguinte informação

>> virtualenv 20.4.2 from /home/atrya/.local/lib/python2.7/site-packages/virtualenv/__init__.pyc
```


## Instalar virtualenv para o Python 3

rode o seguinte código em seu terminal
```
>> pip3 install virtualenv

```
Para verificar se a instalação ocorreu de forma correta, digite o seguinte comando no seu 
terminal:

```
>> virtualenv --version

 //  terá como saída no terminal a seguinte informação

>> virtualenv 20.0.28 from /home/atrya/.local/lib/python3.8/site-packages/virtualenv/__init__.py

```


# Criando uma Virtualenv

Para criar uma virtualenv é muito fácil, basta ir para o diretório do projeto que você deseja 
criar a virtualenv e roda o seguinte comando no seu terminal:

```
// <nome > é o nome que você deseja dá a sua virtualenv, normalmente se coloca env.

>> virtualenv <Nome>

 //  Esperi o processo de criação termionar, e você terá a sua primeira virtualenv

```
Depois de rodado o código assim, você irá ver no diretório do seu projeto uma nova pasta
com o nome que você colocou em sua virtualenv

até esse nomento, nós criamos a env, no entanto, para podemos utilizala devemos ativar-la
para isso demos correr o seguinte código no termial aberto na pasta do projeto.

```
// env deve ser trocado apara o nome que vocẽ deu a pasta da sua virtualenv.

>> source env/bin/activacte

```
pronto, agora você tem sua virtualenv ativada e pronta para ser utilizada em seu projeto, agora todo pacote/lib/módulo que você instalar utilizando o pip irá ser instalado em sua virtalenv e estará disponível para esse projeto em explecifico.

lembrando que caso você feche o terminal, e volte para dá continuidade em seu projeto você deve ativar sua virtualenv novamente seguindo o passo anterior.

# Desativando e removendo Virtualenv

caso você não deseje mais utilizar uma env, voçê pode desativar ou remove-la/deletar-la.
Para desativa-lá basta fechar o terminal ou digitar no terminal o seguinte copmando:

```
>> deactivate

```
Caso você deseje remove-lá para sempre, digite o seguinte comando no terminal, denttro do diretório do projeto:

lembrabdo de modificar o < env > pelo nome que você deu a sua env. 

```
>> rm -r env
```

<div class="embad">

<iframe width="100%" height="400" src="https://www.youtube.com/embed/Osd7hcts8RQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen=""></iframe>

</div>

Esperamos tê-lo(a) ajudado(a) a sanar suas dúvidas.
Até o próximo post...
