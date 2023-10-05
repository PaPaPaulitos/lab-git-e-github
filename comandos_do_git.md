# Comandos do Git

Já vimos esses comandos em [Criando seu primeiro repositório](./criando_seu_primeiro_repo.md), mas eles também vão estar aqui.

### Para iniciar o *Repositório local* digite o seguinte comando:

```bash
git init
```

---

### Ligando um *Repositório local* a um remoto

> Faça o login do GitHub caso necessário

```bash
git remote add origin [LINK DO SEU REPOSITORIO]
```

---

### Atualizando um *Repositório local*

```bash
git add [CAMINHO DO QUE QUER JOGAR NO REPOSITÓRIO LOCAL OU . PARA ADICIONAR TODOS ARQUIVOS QUE FORAM ALTERADOS ]
```

---

### Realizando um *commit* local.

> Um commit é a realização permanente de um conjunto de tentativas de alteração, marcando o fim de uma transação e fornecendo durabilidade às transações ACID.

```bash
git commit -m "DIGITE AQUI A SUA MENSAGEM"
```

---

### Enviando o *commit* também para o GitHub pela primeira vez

Vamos criar uma Branch chamadada master no GitHub

```bash
git push --set-upstream origin master
```

**Observação apartir do momento que você da o comando acima você só precisa digitar**

```bash
git push
```

**Enviando a atualização para uma Branch específica**

```bash
git push [NOME DA BRANCH]
```

---

### Atualizando o seu *Repositório Local* trazendo as modificações do *Repositório Remoto*

```bash
git pull
```

**Atualizando o seu *Repositório Local* trazendo as modificações do *Repositório Remoto* com base em uma Branch**

```bash
git pull [NOME DA BRANCH]
```

---

### Baixando um *Repositório Remoto* da internet

```bash
git clone [LINK DO REPOSITORIO]
```


---

### Alterando o nome branch atual

```bash
git branch -M main
```

---

Nesse caso mudamos o nome da Branch de *master* para *main*

### Verificando o status do *Repositório Remoto*

```bash
remote -v
```

---

### Vendo a lista de modificações em um *Repositório Local*

```bash
git status
```

---

### Removendo todas alterações de um *Repositório Local*

```bash
git reset
```

**Verificando o ID dos *commits***

```bash
git log
```

**Voltando um commit temporariamente**

```bash
git checkout <id>
```

> Quando voltamos um commit temporariamente, nós não alteramos o repositório.


**Deletando todos commits a partir de uma data**

```bash
git reset --hard <id>
```

> Nesse caso vamos voltar o repositório para o commit que selecionamos.

---

### Jogando o conteúdo da sua Branch atual para outra

```bash
git merge [NOME DA BRANCH]
```

---

### Criando uma nova Branch

```bash
git branch [NOME DA BRANCH]
```

**Mudar nome da Branch atual**

```bash
git branch -m [NOME DA BRANCH]
```

**Listar todas as Branchs**

```bash
git branch
```


**Cria uma branch e já te manda para ela**

```bash
git checkout -b [NOME DA BRANCH]
```

**Te redireciona para uma Branch**

```bash
git checkout [NOME DA BRANCH]
```

**Realiza um merge de um arquivo especifico na branch atual**

```bash
git checkout [NOME DA BRANCH QUE VOCÊ QUER O ARQUIVO] [CAMINHO DO ARQUIVO]
```

---