# Trabalhando com versionamento


## Vendo a lista de modificações em um *Repositório Local*

```bash
git status
```

---

## Removendo todas alterações de um *Repositório Local*

```bash
git reset
```

## Verificando o ID dos *commits*

```bash
git log
```

## Voltando um commit temporariamente

```bash
git checkout <id>
```

> Quando voltamos um commit temporariamente, nós não alteramos o repositório.


## Deletando todos commits a partir de uma data

```bash
git reset --hard <id>
```

> Nesse caso vamos voltar o repositório para o commit que selecionamos.