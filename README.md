- [1. guiaLinux](#1-guialinux)
  - [1.1. Diretórios](#11-diretórios)
  - [1.2. Comandos básicos para manipulação de arquivos](#12-comandos-básicos-para-manipulação-de-arquivos)
  - [1.3. Atualizar pacotes no Linux](#13-atualizar-pacotes-no-linux)
  - [1.4. Editores de texto](#14-editores-de-texto)
    - [1.4.1. nano](#141-nano)
    - [1.4.2. vim](#142-vim)
  - [1.5. Gerenciamento de usuários e grupos](#15-gerenciamento-de-usuários-e-grupos)
  - [1.6. Gerenciamento de permissões](#16-gerenciamento-de-permissões)
  - [1.7. REDE](#17-rede)
  - [1.8. Compactar e descompactar arquivos](#18-compactar-e-descompactar-arquivos)


# 1. guiaLinux
Guia de comandos para administração de servidores Linux

## 1.1. Diretórios
~ - pasta home

/ - diretório raiz

bin - arquivos binários

boot - arquivos de inicialização

dev - arquivos entrada e saída do sistema

etc - arquivo de configuração

home - usuários do sistema

lib - arquivo de bibliotecas

media - pasta dos dispositivos

opt - arquivos de aplicações não oficiais do sistema

## 1.2. Comandos básicos para manipulação de arquivos
ls - listar diretórios

cd - serve para mudar de diretórios

cd nome do diretório - muda para o diretório especifico

cd / raiz dos arquivos

cd .. / retornar um diretório

cd - volta para o diretório anterior

cd ~ - vai para a home

cd table - auto completa o nome do diretório

CTRL + ALT + T - abri o terminal no Linux

clear - limpa o terminal

## 1.3. Atualizar pacotes no Linux
sudo apt-get update - atualiza todos os repositórios

sudo apt-get upgrade - atualiza todos os aplicativos

nome do programa + enter - verificar se tem o programa instalado na máquina

sudo apt-get install + nome do programa - instala aplicativos

sudo apt-get purge + nome do programa - instala aplicativos

## 1.4. Editores de texto
### 1.4.1. nano
nano + enter - abre o editor vazio para criar o arquivo

CTRL + O - Salva o arquivo

CTRL + X - Sai do editor

nano + nome do arquivo - abre o editor para editar o arquivo

CTRL + R - cópia dados de um arquivo para outro

### 1.4.2. vim
Vim + nome do arquivo a ser criado - abre o editor vazio para criar o arquivo

I + ENTER - modo de inserção

Esc - sai do modo de inserção

: + X - Salva o arquivo e sai

: + W - Salva o arquivo, mas não fecha o editor

:q - fecha o editor

## 1.5. Gerenciamento de usuários e grupos
sudo + Adduser + nome do usuário - cria um usuário

Ls /home/ - exibi todos os usuários

sudo userdel —remove + nome do usuário a ser deletado - remove um usuário do sistema

sudo usermod -c ‘+ nome do usuário a ser alterado’ + nome do usuário - altera o nome do display

sudo usermod -l + nome do usuário a ser alterado -d /home/ nome alterado -m + nome do usuário antigo

sudo user mod - L + nome do usuário a ser bloqueado - bloqueia a o usuário

sudo user mod - U + nome do usuário a ser bloqueado - desbloqueia a o usuário

getent group - exile todos os grupos criados no sistema

sudo groupadd -g + id do grupo + nome do grupo - cria um grupo

sudo groupdel + nome do grupo - deleta um grupo

groups + nome do usuário - exibi os grupos pertencente ao usuário

sudo usermod -a -G + nome do grupo que o usuário irá + nome do usuário - move um usuário de um grupo para outro

## 1.6. Gerenciamento de permissões
chmod + números das permissões - concede permissão de leitura e escrita em arquivos e diretórios

sudo Chown + nome do usuário + nome do arquivo - muda o dono do arquivo

sudo Chown + nome do usuário: grupo de usuário + nome do arquivo - muda o usuário e o grupo do arquivo

sudo chgrp + nome do grupo que o arquivo vai + nome do arquivo - muda apenas o grupo

CTRL + SHIF + C - copia o conteúdo selecionado

## 1.7. REDE
Conceitos básicos de rede.

TCP - Transfer control protocol - serve para a transmissão de dados de forma segura na internet

UDP - user dataram protocol - serve para a transmissão de dados de forma mais rápida na internet

DNS - o endereço que é digitado para a busca de um site na web

Ping - envio de requisições para verificar se um IP retorna

Netstat - verificar o que o computador está conectado ou recebendo de outros computadores

## 1.8. Compactar e descompactar arquivos
tar -czvf + nome do arquivo.tar.gz + nome do arquivo que será compactado - realiza compactação de arquivos

tar -xzvf + nome do arquivo compactado.tar.gz - descompacta arquivos

tar -xzvf + nome do arquivo compactado.tar.gz -C + nome do diretório - descompacta arquivos em um diretório especifico

zip -r + nome do arquivo .zip + arquivo a ser compactado

unzip -r + nome do arquivo .zip -d + nome do diretório onde será descompactado