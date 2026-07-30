# Infinity Vacation Club — App

Sistema de pontos de férias do Infinity Vacation Club: painel administrativo (desktop) para o vendedor cadastrar clientes e gerenciar destinos/categorias, e um app do cliente (mobile/web) para consultar saldo, resgatar destinos e acompanhar o extrato.

## Sobre o Projeto

O sistema é dividido em duas partes que compartilham os mesmos dados:

- **Painel do vendedor** — programa instalável para Windows (.exe), usado na sala de vendas para cadastrar clientes na hora, gerenciar destinos (com galeria de fotos) e configurar categorias/pontuação.
- **App do cliente** — instalável no celular direto pelo navegador (PWA), onde o cliente faz login com CPF e senha para ver saldo de pontos, resgatar destinos e acompanhar reservas.

## Funcionalidades

### Painel do vendedor (desktop)
- Cadastro de clientes com CPF e senha (senha gerada automaticamente e enviada por e-mail)
- Reenvio de senha / recuperação de acesso por e-mail
- Cadastro de destinos com galeria de múltiplas fotos, dicas de viagem e pontuação por noite
- Configuração de categorias/tiers (Bronze, Prata, Ouro, Diamante)
- Verificação e instalação de atualizações do próprio programa

### App do cliente (mobile/PWA)
- Login com CPF e senha
- Saldo de pontos e categoria do titular
- Busca e resgate de destinos com cálculo de check-in/check-out
- Extrato de pontos e histórico
- Perfil com foto e tema claro/escuro
- Instalação como aplicativo direto do navegador ("Adicionar à tela inicial")

## Tecnologias

- **Electron** — empacotamento do painel do vendedor como programa Windows instalável (.e
- **electron-updater + GitHub Releases** — atualização automática do programa instalado
- **HTML, CSS e JavaScript** (sem framework/build step)
- **Node.js + Nodemailer** — envio de e-mails transacionais (boas-vindas e recuperação de senha) via SMTP
- **PWA** (manifest + service worker) — instalação do app do cliente no celular, hospedad
- Armazenamento local em arquivo (por computador/instalação), sem banco de dados na nuvem

## Objetivo

Proporcionar uma experiência premium aos associados do Infinity Vacation Club, com um painel de vendas ágil para cadastro na hora e um app de pontos moderno, rápido e fácil de instalar no celular.

---

© Infinity Vacation Club
