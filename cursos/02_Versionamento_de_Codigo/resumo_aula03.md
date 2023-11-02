# Primeiros Passos Git & Github

## Clonando Repositórios

Há duas opções para clonagem de repositórios:

1. Transformando um diretório local em um repositório git, através do comando `git init`

``` bash
# Primeiro criamos uma pasta

$ mkdir HelloGit

$ cd HelloGit

$ git init

# Pronto, criado um repositório Git
```

2.Clonando um repositório remoto para sua máquina.

```bash

$ git clone <URL do repositório> 

# Opcionalmente podemos nomear a pasta que vai receber o repositório clonado

$ git clone <URL> <Nome_da_pasta>

```

### Salvando Alterações no Repositório Local | `git add`

Apóis criar um repositório, vamos querer salvar as aletrações de nossos arquivos no processo de versionamento. Para isso, precisaremos subir o que foi feito ao *stagging*. Utilizaremos o comando `git status` para verificar se as alterações estão nesse *stagging* e prontas para serem *commitadas*, isto é, gravadas no controle de versão.

Para adicionarmos ao *stagging*, utilizaremos o comando `git add` para adicionar arquivos à área de preparação, antes de incluirmos os arquivos adicionados a um *commit*.

``` bash
git add <Nome_do_Arquivo>

# Para adicionar todos os arquivos de um diretório

git add .
```

### Listando Commits | `git log`

O comando `git log` irá listar todos os *commits* de um projeto.

### Removendo um Repositório

Para cancelar o monitoramento *git* de uma pasta, é só remover o diretório oculto `.git/` de dentro da pasta. Podemos fazer isso com o comando:

``` bash
rm -rf .git
```

### Retornando a um Estado Anterior | `git restore`

Para recuperar a versão anterior de um ou mais arquivos, executamos o comando:

``` bash
git restore <NOME DOS ARQUIVOS>
```

Para retornar ao estado anterior de toda uma aplicação, digite na raiz:

```bash
git restore .
```

> O comando irá descartar TODAS as alterações feitas e que não tenham sido commitadas

### Alterando Mensagens de Commit | `git commit amend`

Podemos alterar o texto que identifica um *commit*. Para alterar o texto do último commit, devemos utilizar o comando:

```bash
git commit --amend -m "<mensagem que vai substituir a anterior>"
```

### Retornando ao estado de um Commit Anterior | `git reset`

O comando `git reset` irá retornar o estados dos seus arquivos ao de um *commit* anterior. Há três opções de restauração:

- Utilizando a flag `--soft`: Após copiar o *hash* do *commit* que se quer restaurar, devemos digitar o comando abaixo, para restaurar o estado dos arquivos nesse *commit*:

```bash
git reset --soft <hash do commit>
```

## Trabalhando com Branches

A tradução de *branch* é ramo. Ou seja, quando criamos branches estamos ramificando nosso projeto e essa ideia de ramificação é precisa para ilustrar que ramificações dentro de ramificações vão criando um complexo sistema em um projeto, que o *git* contribui para controlar.
