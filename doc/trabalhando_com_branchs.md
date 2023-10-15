# Trabalhando com Branchs


Criar uma *Branch* é criar uma ramificação de um código, ou seja a partir de um commit, você cria uma versão *paralela* desse código.

![Criando uma Branch](./Imagens/trabalhando_com_branchs_1.png)

Isso serve justamente para que os programadores possam produzir em paralelo e depois juntar esses códigos fazendo o que chamamos de *merge*.

![Fazendo um Merge](./Imagens/trabalhando_com_branchs_2.png)

## Criando uma nova Branch

```bash
git branch [NOME DA BRANCH]
```

---

## Mudar nome da Branch atual

```bash
git branch -m [NOME DA BRANCH]
```

---

## Listar todas as Branchs

```bash
git branch
```

---

## Alterando o nome branch atual

```bash
git branch -M [NOME QUE QUER DAR PARA A BRANCH]
```

---

## Jogando o conteúdo da sua Branch atual para outra

```bash
git merge [NOME DA BRANCH]
```

---

## Cria uma branch e já te manda para ela

```bash
git checkout -b [NOME DA BRANCH]
```

---

## Te redireciona para uma Branch

```bash
git checkout [NOME DA BRANCH]
```

---

## Realiza um merge de um arquivo especifico na branch atual

```bash
git checkout [NOME DA BRANCH QUE VOCÊ QUER O ARQUIVO] [CAMINHO DO ARQUIVO]
```

---