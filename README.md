# Fliperama CIABA

Jogos rápidos de conta, palavra e inglês para a galera: Quiz da Galera, Tiro Certo, Duelo de Tabuada, Forca em equipe, Stop e 5 clássicos. Tem login com Google, chat moderado, ranking por jogo e salas ao vivo.

## Como está montado
- `index.html`: o jogo inteiro, com a página e o código num arquivo só. É publicado pelo GitHub Pages.
- `config.js`: a configuração do projeto Firebase, mais o e-mail de quem modera.
- `database.rules.json`: as regras de segurança do banco. Elas são coladas no Firebase, em Realtime Database > Regras.

## O que as regras garantem
- Só quem entrou com o Google lê e grava.
- Cada pessoa só altera o próprio perfil e as próprias mensagens.
- Só o moderador (contato@marcionagano.com) altera a moderação, bane alguém ou vê os e-mails.
- Quem for banido não grava mais nada.

O código-fonte fica na pasta de trabalho do Claude: `build_github.py` gera esta pasta.
