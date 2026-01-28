# Git para leigos

## Índice
*   [Introdução](#introdução)
*   [O que é Git?](#o-que-é-git)
*   [Primeiros Passos](#primeiros-passos)
*   
*


# Introdução
Este repositório é destinado a pessoas que estão dando os primeiros passos no Git e no versionamento de código.

O objetivo é explicar, de forma simples e direta, como funcionam os principais comandos do Git e para que cada um deles serve.

A ideia desse repositório surgiu da necessidade de aprender Git de uma vez por todas e também de criar um material de consulta para quando bater a dúvida ou o esquecimento sobre algum comando específico.

# O que é Git?
O Git é um sistema de controle de versão criado por volta de 2005. Sua origem está relacionada a um conflito entre a comunidade que desenvolvia o núcleo do Linux e a empresa responsável pelo BitKeeper, ferramenta de versionamento utilizada na época, que deixou de ser gratuita.

Diante dessa situação, Linus Torvalds, criador do Linux, decidiu desenvolver uma nova ferramenta que atendesse às necessidades da comunidade: rápida, distribuída e de [código aberto](https://aws.amazon.com/pt/what-is/open-source/).

# O que é, de fato, o Git e como ele funciona?

Como foi dito, Git é um controlador de versionamento [open-source](https://aws.amazon.com/pt/what-is/open-source/). Com ele, você controla a versão do seu código, projeto ou trabalhos.

Vamos imaginar o seguinte cenário, separando o problema e a solução:

Você está em sua casa desenvolvendo uma aplicação onde tem diversas linhas de código já prontas, mas falta energia do nada e seu computador queimou. Você não tem o projeto salvo em um pendrive e tem até o dia seguinte para apresentar o [MVP](https://www.rdstation.com/blog/marketing/mvp-minimo-produto-viavel/) do seu projeto ao cliente. E agora?

Com o Git, você consegue fazer o versionamento do seu projeto, salvando-o em alguma plataforma como o [GitHub](https://github.com/), e pode acessá-lo de qualquer computador ou até visualizar o seu código online. Com o Git, você tem todo o controle de versão do seu projeto e pode recuperar algum código que tenha apagado por qualquer motivo, pode realizar [commits](), criar novas [branches]() e até trabalhar em conjunto com uma equipe no mesmo projeto e na mesma linha de código. Incrível, né? Agora vamos aos primeiros passos de como utilizar essa belezinha.

# Primeiros passos
Para começar a usar a ferramenta, precisamos concluir dois passos principais, que são instalar o Git e ter uma conta em alguma plataforma de hospedagem de repositório Git.

## Criando uma conta no GitHub
O GitHub é uma plataforma online usada para hospedar repositórios Git, permitindo salvar, compartilhar e colaborar em projetos de código. Ele será utilizado aqui para armazenar o projeto versionado e facilitar o acesso de qualquer lugar.
Crie uma conta em uma plataforma web de hospedagem. Neste tutorial, vou utilizar o GitHub.

1. Entre na home do [GitHub](https://github.com/):

![HomeGitHub.png](assets/images/HomeGitHub.png)

2. Clique em **Criar uma conta**

![CreateAccount.png](assets/images/CreateAccount.png)

3. Com a conta criada, você terá acesso ao Dashboard. Entre na aba de perfil. Nessa página, você poderá visualizar todas as atividades realizadas no GitHub.

![profile-github.png](assets/images/profile-github.png)

**Ótimo, agora temos o Git instalado e uma conta no GitHub para começar a desenvolver!**

## Criando um repositório

Com uma conta no GitHub, vamos criar um repositório. Basta acessar seu perfil GitHub e acessar a aba repositórios e clicar em **New**.

![New.png](assets/images/new.png)

Para criar um repositório, vamos precisar adicionar um nome a ele, adicionar se ele será público ou privado e se queremos ou não adicionar um README, que é um documento de texto, normalmente é utilizado para adicionar explicações sobre o projeto.

![createRepository.png](assets/images/createRepository.png)

Com o repositório criado vamos ter acesso ao link de clonagem para a maquina local

![repository.png](assets/images/repository.png)


## Instalando o Git na maquina

Para instalar, basta acessar:
* Este link para [instalação do Git no Windows](https://git-scm.com/)
* Este link para [instalação do Git no Linux](https://git-scm.com/install/linux)
* Este link para [instalação do Git no Mac](https://git-scm.com/install/mac)

## Configurando o git na maquina local

No seu computador, abra o terminal de comando

### Tutorial de linha de comando

A linha de comando é a principal forma de interagir com o sistema operacional, vamos primeiro nos familiarizar com ela antes de continuar.
Vamos usar alguns comandos. É importante saber que dependendo do sistema que está executando seja Windows ou Mac, os comandos podem ser diferentes. Porem, linux e o mac possuem o mesmo gerenciador de pacotes *nix, portanto podem ter os mesmos comandos.

| \\*nix (Linux / macOS) | Windows    | O que faz |
|:----------------------:|:----------:|:----------|
|         `pwd`          | `echo %cd%`| Mostra o diretório atual (onde você está). |
|          `ls`          | `dir`      | Lista arquivos e pastas do diretório atual. |
|          `cd`          | `cd`       | Navega entre diretórios. |
|          `cp`          | `copy`     | Copia arquivos de um local para outro. |
|          `mv`          | `move`     | Move ou renomeia arquivos e pastas. |
|          `rm`          | `del`      | Remove arquivos. |
|        `rm -r`         | `rmdir /s` | Remove diretórios e seus conteúdos. |
|        `mkdir`         | `mkdir`    | Cria um novo diretório. |
|        `clear`         | `cls`      | Limpa a tela do terminal. |
|          `.`           | `.`        | Representa o diretório atual. |
|          `..`          | `..`       | Representa o diretório pai (um nível acima). |


## Definir variaveis globais git

Quando formos utilizar o git, vamos precisar realizar commits, e precisamos rotular esses commits pára que e possamos saber quando ele foi feito e por quem.

**Diga ao git seu nome:**
```bash
git config --global user.name "YOUR NAME"
```

**Diga ao git o seu endereço de e-mail:**
```bash
git config --global user.email "YOUR EMAIL ADDRESS"
```
Ótimo agora estamos prontos para subir nosso código!

