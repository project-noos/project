# Noos

Noos é proposta de projeto de sistema operacional baseada em linux usando tecnologia web

## Objetivos

Objetivo seria criar um sistema operacional de codigo livre e de fácil usabilidade com interface com janelas, fosse focada no navegador assim como Chrome OS, porem também possibilitado a instalação de aplicações de terceiros.

## Gerenciador Sistema

O gerenciador do sistema seria feito gotty

## Gerenciador de Janelas

O gerenciador de janelas seria traves react js rodando as aplicações dentro webview.

## Aplicações base

Para ter uma versão minima é necessário um conjunto mini de aplicações já pre instaladas, como terminal, gerenciador de arquivos e editor de texto.

No GitHub existe repositório com nome [electron-sample-apps](https://github.com/hokein/electron-sample-apps) com exemplos de plicações simples mais muito útil para sistema base.

## Aplicações de Terceiros

Teria que ser devolvido uma build específico para aplicações atuais em Electron js.
Como o Sistema é uma renderização do navegador as aplicações teriam duas possibilidades, roda como componentes ou como webview.

Para os programas tradicionais de linux uma solução seria transmitir a janela do programa via vnc para localhost para ser aberto no navegador.

- [CloudTk](https://wiki.tcl-lang.org/page/CloudTk)

## Problemas

- Compartilhamento de memoria entre processos
- Navegador web tem está junto gerenciador de janelas
- Syscall
- Retrocompatibilidade com programas antigos
    - [https://github.com/linuxserver/docker-baseimage-rdesktop-web](https://github.com/linuxserver/docker-baseimage-rdesktop-web)
    - [https://github.com/linuxserver/docker-firefox](https://github.com/linuxserver/docker-firefox)
    - [https://wiki.tcl-lang.org/page/tkEngine](https://wiki.tcl-lang.org/page/tkEngine)

## Vantagens

- Retrocompatibilidade entre programas em Electron JS e WebApps
- Navegador de internet super leve
- Bonito / Personalizável
- Suporte ao Windows e Linux
- Nova forma de desenvolvimento para desktop
    - funções lambda
    - Api compartilhada

## Referencia

[https://demo.os-js.org/](https://demo.os-js.org/)

```bash
# interface
npx electron@latest https://google.com

# desktop
npx create-react-app my-app

# terminal
./gotty -w tmux

# arquvios
backend go
https://github.com/filebrowser/filebrowser

# editor texto
https://github.com/gitpod-io/openvscode-server/
```
