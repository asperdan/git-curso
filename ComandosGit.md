**Instalando o Git**
1. Realizar downlod do instalador em:
    - https://git-scm.com/downloads

2. Configurando git global :
    # Verificar a versão do git
    - git --version
    - git config --global user.name "Luis Claudio"
    - git config --global user.email "luiscla1987@gmail.com"
    - git config user.name
    - git config user.email
    - git config --list
3. Incializando um repositório:
    - Criar uma pasta
    - mkdir git-repositorio
    - cd git-repositorio
    - git init
4. Ciclo de vida dos arquivos:
    - untracked - O git ainda não conhece o arquivo
    - unmodified - Existe no git mas não foi modificado
    - modified - Modificado 
    - staged - Pronto cria uma versão e volta para o unmodified
5. Ciclos de vida:
 - git status
 - git add Readme.md
 - git commit -m "Add Readme.md"
6. Visualizar logs:
    - git log
    - git log --author="Luis"
    - git shortlog 
    - git shortlog -sn
    - git log --graph
    - git show #hash#
7. Visualizando o diff:
    - git diff
    # somente o nome do arquivo
    - git diff --name-only
    # commitar arquivo que já existe
    - git commit -am "Edit Readme.md"
8. Desfazendo coisas:
    # sem add no sataged
    - git checkout Readme.md
    # adicionado no staged 
    - git reset HEAD Readme.md
    # commitado --soft --mixed
    - git reset --hard #hash anterior#
10. Ligando o repositório local a um remoto:
    - git remote add origin ..
    - git remote
    - git remote -v 
    - git push -u origin main   #explicar da master