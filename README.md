# Guia Completo do Git

## Iniciando um novo repositório

echo "# exemplo_git" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/mistickesterio/exemplo_git.git
git push -u origin main

**Explicação:**
- `git init`: Inicia um novo repositório Git.
- `git add README.md`: Adiciona o arquivo README.md ao índice para ser rastreado.
- `git commit -m "first commit"`: Confirma as alterações feitas e adiciona uma mensagem descritiva.
- `git branch -M main`: Renomeia a branch para "main".
- `git remote add origin <url>`: Conecta o repositório local a um repositório remoto.
- `git push -u origin main`: Envia as alterações para o repositório remoto.

## Conectando-se a um repositório remoto existente

git remote add origin https://github.com/mistickesterio/exemplo_git.git
git branch -M main
git push -u origin main

**Explicação:**
- `git remote add origin <url>`: Adiciona um repositório remoto chamado "origin".
- `git branch -M main`: Renomeia a branch para "main".
- `git push -u origin main`: Envia as alterações locais para o repositório remoto.

## Atualizando seu repositório local

git pull

**Explicação:**
- `git pull`: Atualiza o repositório local com as últimas alterações do repositório remoto.

## Verificando o status do seu repositório

git status

**Explicação:**
- `git status`: Mostra o estado atual do repositório, indicando quais arquivos foram modificados, adicionados ou removidos.

## Configurando suas informações de usuário

git config --global user.email "seu email"
git config --global user.name "seu nome"

**Explicação:**
- `git config --global user.email "seu email"`: Configura o endereço de e-mail associado às suas alterações no Git.
- `git config --global user.name "seu nome"`: Configura o nome associado às suas alterações no Git.

## Clonando um repositório existente

git clone https://github.com/mistickesterio/exemplo_git.git

**Explicação:**
- `git clone <url>`: Cria uma cópia local de um repositório remoto.

## Verificando a versão do Git instalada

git --version

**Explicação:**
- `git --version`: Exibe a versão do Git instalada.

## Visualizando histórico de alterações

git log

**Explicação:**
- `git log`: Mostra o histórico de commits do repositório.

## Ramificação de código

git branch <nome_da_ramificação>
git checkout <nome_da_ramificação>

**Explicação:**
- `git branch <nome_da_ramificação>`: Cria uma nova ramificação.
- `git checkout <nome_da_ramificação>`: Muda para a ramificação especificada.

## Mesclando ramificações

git merge <nome_da_ramificação>

**Explicação:**
- `git merge <nome_da_ramificação>`: Mescla uma ramificação ao código principal.

## Ignorando arquivos

Crie um arquivo chamado .gitignore e adicione os nomes dos arquivos a serem ignorados.

## Removendo arquivos do repositório

git rm <nome_do_arquivo>

**Explicação:**
- `git rm <nome_do_arquivo>`: Remove um arquivo do repositório.

## Desfazendo alterações

git checkout <nome_do_arquivo>

**Explicação:**
- `git checkout <nome_do_arquivo>`: Desfaz as alterações feitas em um arquivo.

## Desfazendo commits

git revert <hash_do_commit>

**Explicação:**
- `git revert <hash_do_commit>`: Desfaz um commit específico.

## Desfazendo commits localmente

git reset HEAD~1

**Explicação:**
- `git reset HEAD~1`: Desfaz o último commit localmente.

## Fazendo tags

git tag v1.0.0 -m "entrega"
git tag -n
git push origin entrega

**Explicação:**
- `git tag v1.0.0 -m "entrega"`: Cria uma tag chamada v1.0.0.
- `git tag -n`: Lista as tags existentes.
- `git push origin entrega`: Envia a tag "entrega" para o repositório remoto.

## Conectando no repositório sem precisar baixar

git remote add origin https://github.com/mistickesterio/exemplo_git.git
git branch -M main
git push -u origin main

**Explicação:**
- `git remote add origin <url>`: Adiciona um repositório remoto chamado "origin".
- `git branch -M main`: Renomeia a branch para "main".
- `git push -u origin main`: Envia as alterações locais para o repositório remoto.

## Gerenciando tags

git tag -a v1.0.0 -m "Versão 1.0.0 - Entrega inicial" <hash_do_commit>
git tag -n
git push origin v1.0.0

**Explicação:**
- `git tag -a v1.0.0 -m "Versão 1.0.0 - Entrega inicial" <hash_do_commit>`: Cria uma tag anotada.
- `git tag -n`: Lista as tags existentes.
- `git push origin v1.0.0`: Envia a tag para o repositório remoto.

## Gerenciando tags final

git clone https://github.com/Thiago163/pim.git
cd pim
git fetch origin --tags
git tag -a v1.0.0 -m "Versão 1.0.0 - Entrega inicial"
git push origin v1.0.0

**Explicação:**
- `git clone <url>`: Clona um repositório remoto.
- `git fetch origin --tags`: Obtém as tags do repositório remoto.

- git tag -a v1.0.0 -m "Versão 1.0.0 - Entrega inicial": define um nome para a tag e da um commit

- git push origin v1.0.0 envia a tag para o GitHub

Lembre-se de que a ordem e a necessidade de cada comando podem variar dependendo da situação em que você se encontra no uso do Git.

