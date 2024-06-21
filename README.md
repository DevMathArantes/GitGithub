Link git-hub
https://github.com/

Link Vercel
https://vercel.com/

Link download do git
https://git-scm.com/downloads

Link com instruções para gerar uma chave SSH
https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

Link para configurações da chave SSH
https://github.com/settings/keys

Link com guia para o git
https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git

Link guia sobre projetos Open Source
https://www.alura.com.br/artigos/open-source-uma-breve-introducao

Link de ferramenta útil ao gitignore
https://www.toptal.com/developers/gitignore

Para descrever o projeto, utilize um arquivo chamado README.md aonde ficará a docummentação do projeto

Para criar arquivos que não devem estar no repositório, basta adiciona-los ao .gitignore (
    Para pastas: NOME/
    Para arquivos: NOME.TIPO
    Para tipos: *.TIPO
)

Indicadores git

    M: A letra M representa o estado Modified, do português modificado. Isso significa que o arquivo já existia no 
    repositório, mas que recebeu alguma modificação que ainda não foi registrada no Git.

    U: A letra U representa o estado Untracked, do português não rastreado. Isso significa que o arquivo ainda não 
    existia no repositório e que ainda não teve seu registro (commit) feito no Git.

    Resolução de confiltos:
   
        Accept Incoming: aceita modificações oriundas do remoto

        Accept Combination Incoming First: realiza a combinação com as linhas do código do repositório remoto no 
        topo.

        Ignore: ignora as modificações.

        Accept Current: Aceita a modificação local no resultado do documento

        Accept combination Current First: Aceita a combinação local + remoto, comprovando que o código local é inserido 
        primeiro que o remoto.

        Ignore: ignora as modificações no resultado no final.

Comandos isolados:

    Mostrar mudanças                         git status
    Mostrar commits do projeto e autores     git log
    Mostrar os repositórios locais           git remote
    Mostrar versões                          git reflog
    Desfaz as mudanças do commit             git revert
    Excluir commit                           git reset --hard ID_DO_COMMIT_ANTERIOR
    Renomear commit                          git commit --amend -m "RENOMEAR"

1- Instalar o git 

2- Abrir o terminal da pasta desejada

3- Utilizar os seguintes comandos: 

    Inicializando                            git init
    Tentando adicionar os arquivos           git add .
    Tentando dar o commit                    git commit -m " NOMEAR "
    Configurando o usuário                   git config --global user.email " EMAIL " 
    Configurando o nome de usuário           git config --global user.name " NOME "
    Direcionando para o repositório          git remote add origin URL_REPOSITÓRIO
    Tentando subir a versão                  git push
    Verifição final                          git push --set-upstream origin master

4- Atualizando mudanças:

    Carregar mudanças(Caso esteja em equipe) git pull
    ...desevolvimento de novas mudanças...
    Adicionando mudanças                     git add .
    Nomeando versão                          git commit -m " NOMEAR "
    Subindo nova versão                      git push
    
5- Coletando projeto em outro dispositivo (necessita de permissão de colaborador)

    Clonando projeto                         git clone URL_REPOSITÓRIO
    ...Desenvolvimento...Atualização padrão (passo 4).