# OB Framework

Framework independente para servidores FiveM na versao GTA V Enhanced.

Este repositorio preserva o codigo-fonte do projeto OB Framework. Ele inclui o
nucleo da framework, banco de dados, inventario, personagens, administracao,
HUD, organizacoes, empregos, economia, veiculos e sistemas de roleplay.

> O projeto esta pausado e esta versao e disponibilizada como arquivo publico.
> Revise e teste tudo em um ambiente separado antes de usar em producao.

## Como funciona

O `server.cfg` inicia primeiro a infraestrutura principal:

1. `ob_database` e `ob_lib` fornecem banco e utilitarios.
2. `ob_core` gerencia sessao, personagem e integracoes centrais.
3. `ob_target`, `ob_inventory`, `ob_vehiclekeys` e voz fornecem os sistemas base.
4. `ob_admin`, `ob_adminmenu`, `ob_editor`, `ob_creator`, `ob_multichar` e
   `ob_spawn` cuidam da administracao e entrada do jogador.
5. As colecoes `[system]`, `[scripts]`, `[maps]`, `[props]` e `[cars]` carregam
   os demais recursos.

Entre os modulos incluidos estao lojas, banco, garagem, combustivel, telefone,
organizacoes, policia, mecanica, clima, HUD, pause menu, trabalhos legais,
plantacoes, venda de drogas, evidencias, lavagem de dinheiro e roubos.

## Requisitos

- FXServer compativel com GTA V Enhanced;
- MariaDB/MySQL;
- OneSync;
- Git LFS somente se voce tambem clonar o repositorio de imagens;
- configuracao privada valida do Cfx.re, banco e servicos externos.

## Instalacao

1. Clone este repositorio na pasta desejada do servidor.
2. Copie `server.private.cfg.example` para `server.private.cfg` e substitua os indicadores, como
   `CFX_KEY`, `LOGIN`, `SENHA`, `HOST`, `NOME_DO_BANCO` e `FIVEMANAGE_KEY`.
3. Configure `SEU_IDENTIFICADOR` e os demais indicadores do `server.cfg`.
4. Importe ou deixe os recursos criarem o esquema de banco exigido.
5. Baixe o repositorio de imagens e publique seu conteudo no caminho `/orbis/`.
6. Inicie pelo `server.cfg` e acompanhe o console na primeira inicializacao.

## Imagens obrigatorias

Os assets das interfaces foram separados para evitar que o repositorio da
framework fique com mais de 2 GB. Baixe-os em:

**[OB-Framework-Imagens](https://github.com/obframework/OB-Framework-Imagens)**

O conteudo desse repositorio deve ser servido por HTTP/HTTPS sob `/orbis/`.
Sem ele, veiculos, itens, roupas e outras imagens das interfaces podem ficar
ausentes.

## Seguranca

O repositorio contem apenas o arquivo de exemplo com indicadores. Nunca publique seu
`server.private.cfg` preenchido, tokens, senhas, chaves Cfx, webhooks ou dados
reais de banco. Para producao, mantenha os valores privados fora do Git.

## Versao Legacy

Para GTA V Legacy, use o repositorio
**[OB-Framework-Legacy](https://github.com/obframework/OB-Framework-Legacy)**.

## Licencas

Os recursos de terceiros mantem suas respectivas licencas e creditos. Antes de
redistribuir ou operar comercialmente, confira cada recurso individualmente.
