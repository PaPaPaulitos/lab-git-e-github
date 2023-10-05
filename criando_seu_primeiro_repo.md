# Criando o seu primeiro repositório

## Pré-requisitos

- Baixar o [Git](./baixando_o_git.md)

- Ter uma conta no [GitHub](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home)

## Criando o Repositório no GitHub

- Clique no botão de **+** no canto superior direto no GitHub.

![Criando Repo](./Imagens/criando_repo_1.png)

- Clique em **New repository**

![Criando Repo](./Imagens/criando_repo_2.png)

## Explicando os campos

### *Repository template*

Serve caso você queira reutilizar o template de outro repósitorio, como exemplo um repósitorio configurado com o Google Colab para ciência de dados, normalmente não utilizar esse campo, então deixamos o **Default** que é **No template**.

![Repository template](./Imagens/criando_repo_3.png)

Mostrando as opções desse campo

![Owner_options](./Imagens/criando_repo_6.png)

### *Owner*

Esse campo é para decidir se o Repositório vai ser seu ou de alguma organização que você faz parte.

![Owner](./Imagens/criando_repo_4.png)

Mostrando as opções desse campo

![Owner_options](./Imagens/criando_repo_5.png)

### *Repository name e Description*

São os campos que vão dar o nome e a descrição do repositório no seu GitHub ou da organização, sendo descrição *opcional*, pois nossa documentação vai ser feita usando *MarkDown*

![Repository name e Description](./Imagens/criando_repo_7.png)

Mostrando aonde aparece esses campos em um Repósitorio.

![Repository name e Description](./Imagens/criando_repo_8.png)

### *Visibilidade*

Sendo os campos mais importantes eles funcionam da seguinte forma:

- *Public*: Ao marcar esse campo o seu repositório vai estar visivel para todos usuários do GitHub.

- *Private*: Ao marcar esse campo o seu repositório vai estar visivel para você e todos a quem você conceder acesso.

> É interessante começar todos repositórios como privado e depois mudar a sua visibilidade para público.

![Visibilidade](./Imagens/criando_repo_9.png)

### *add a README file*

É interessante deixar essa opção marcada, pois é mais fácil de documentar escrevendo um **MarkDown**, temos uma sessão só sobre esse assunto nessa apostila.

> Inclusive essa apostila que você está lendo foi escrita em **MarkDown**

![README](./Imagens/criando_repo_10.png)

### *Add .gitignore*

O arquito *.gitignore* faz com que a nós possamos reduzir o tempo e espaço na hora de subir um repositório, só deixando arquivos essenciais para executar um código, ignorando arquivos binários como *.exe*, *node_modules* em JavaScript, *venv* e *pycache* em Python e assim por diante.

> É interessante você já escolher um template de .gitignore se souber a linguagem que vai trabalhar

![README](./Imagens/criando_repo_11.png)

### *Choose a license*

Essa opção é mais caso você queira dar uma licença já existente pro seu software, a mais utilizada é a do [*MIT* para programas *Open Source*](https://www.diegobrocanelli.com.br/open-source/a-licenca-mit/).

### Iniciando o Repositório

Agora com os dados cadastrados conforme a necessidade podemos clicar no botão **Create repository**

![Criando Repositorio](./Imagens/criando_repo_12.png)

---

## Criando Repositório local e conectando ele ao GitHub

- Crie uma pasta no seu computador com o nome do projeto

- Entre na pasta, clique com o botão direito e clique em *Git Bash Here*.

![Git Bash here](./Imagens/criando_repo_13.png)

- Ela vai abrir essa tela.

![Git Bash](./Imagens/criando_repo_14.png)

- Para iniciar o *Repositório local* digite o seguinte comando:

```bash
git init
```

- Agora para conectar ele ao GitHub use o seguinte comando:

> Faça o login do GitHub caso necessário

```bash
git remote add origin [LINK DO SEU REPOSITORIO]
```

- Adicione ao Repositorio para testa-lo

![Git Bash](./Imagens/criando_repo_15.png)

- Digite o seguinte comando para jogar as mudanças no *Repositório local*

```bash
git add .
```

- Digite uma mensagem para o *commit*

> Um commit é a realização permanente de um conjunto de tentativas de alteração, marcando o fim de uma transação e fornecendo durabilidade às transações ACID.

```bash
git commit -m "DIGITE AQUI A SUA MENSAGEM"
```

- Envie o *commit* também para o GitHub

```bash
git push --set-upstream origin master
```

> Observação apartir do momento que você da o comando acima você só precisa digitar

```bash
git push
```

- Verifique o GitHub

![Git Bash](./Imagens/criando_repo_16.png)
