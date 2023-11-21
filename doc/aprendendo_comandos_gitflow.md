# Aprendendendo Comandos GitFlow

## Para Iniciar o GitFlow no seu Repositório
 Para iniciarmos o gitflow em nosso repositório utilizamos o seguinte comando
 - git flow init
> Após isso, será iniciado as duas branches padrões do Git Flow

- master - Ambiente de produção
- develop - Ambiente de Desenvolvimento

´Após isso já estamos prontos para utulizar os comandos git flow em nosso repositório´.

## Como Iniciar uma Feature ?

Para iniciar uma Feature usaremos o seguintes comando

### ´git flow feature start 'nome da feature'´

Após executar esse comando, será criando uma branch ´LOCAL´ baseada na develop para que você realize as alterações necessária, como na imagem Abaixo:

![Feature](./Imagens//Feat%20+%20DEvelop%20(1).png)

Depois de ralizarmos todas as alterações, devemos finalizar a ´feature´, para finaliza-la usaremos os  seguintes comandos:

- ´git add .´ -  como vimos anteriormente nos comandos básicos de git.

- ´git commit -m ""´ -  que também vimos anteriormente.

## Como Finalizar uma Feature ?

Para finalizarmos, utilizaremos o seguinte comando

### ´git flow feature finsh  'nome da feature'´

Após executar este comando, a branch ´LOCAL´ criada será deletada e será feito o ´MERGE´ na branch ´DEVELOP´ e você será redirecionado automáticamente
para a branch ´DEVELOP´

## E como geramos uma versão do nosso código ?

Para gerarmos uma versão de produção do nosso código, utilizaremos o seguinto comando

### ´git flow release start 'nome da release'´

Ao executar essa esse comando será iniciando uma branch, como demostrado abaixo:

![Release](./Imagens/DEV%20+%20RELEASE%20+%20MASTER%20(1).png)

Até aqui tudo certo?!!

Agora precisamos publicar essa versão, Para isso, utilizamos o seguinte comando:


### ´git flow release public 'nome da release'´

Após executado, ele publica a release no repositório remoto, tornando-a uma candidata e consequentemente realizar ´DEPLOY´ em ´PRÉ-PROD´

> AGORA PRECISAMOS FINALIZAR UMA VERSÃO

Para isso utilizamos o seguinte comando

### ´git flow releaser finish 'versao'´


No momento que finalizar, o git abre em sequência três editores de texto:

- O primeiro é relacionado ao merge da branch release v1.0.0 com a Master, que você pode detalhar o que contempla esta release.
- O segundo é relacionado tag, para facilitar a mudança e identificação, incluir a tag da versão que estão indo para produção v1.0.0
- Por ultimo o merge da release com com a Develop.

![Release-2](./Imagens/release%20gitflow1.png)

## Subimos código com erro em produção E AGORA COMO CORRIGIR ?

Sabemos que é muito normal subirmos códigos com erro em produção, pensando nisso foi desenvolvido uma ferramente própria pra isso.

> E para isso, usamos o seguinte comando.

### ´git flow hotfix start 'nome do hotfix'´

Após o comando ser executado, é aberto uma branch ´HOTFIX´, como vemos na imagem abaixo:

![HotFix](./Imagens/Master%20+%20Hotfix%20+%20Develop%20(1).png)

Nessa branch você corrigirá todos os erros encontrados em produção e após isso você irá fecha-lá, mas ates exxecutará os seguintes comandos:

- ´git add .´ -  como vimos anteriormente nos comandos básicos de git.

- ´git commit -m ""´ -  que também vimos anteriormente.

> AGORA SIM PODEMOS FINALIZAR NOSSO ´HOTFIX´

E para finaliza-lô, executaremos o seguinte comando:

### ´git flow hotfix finish -n 'nome do hotfix'´

Após executar o comando, automáticamente a branch será fechada e ´MERGEADA´ nas suas branches em uso ´MASTER´ e ´DEVELOP´.

# ARVORE DO GIT FLOW

![ÁRVORE-GIT-FLOW](./Imagens/arvore%20git%20flow%20(1).png)
