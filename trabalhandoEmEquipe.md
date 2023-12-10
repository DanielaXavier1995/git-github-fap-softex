## 🛠️ Trabalhando em equipe com o Git e GitHub:


                          🤔 COMO PODEMOS UTILIZAR O GIT E GITHUB PARA TRABALHAR EM EQUIPE? 🤔

### 1° PASSO:
Utilizar o fork para trazer uma cópia do repositório principal para a sua conta do GITHUB.

### 2° PASSO: 
**Clonar o projeto**.

                             ❗ Voçê deve clonar o projeto (fork) da sua conta do GITHUB ❗ 

### 3° PASSO: 
*Linkar o projeto ao repositório remoto de origem (UPSTREAM)

                                                 git remote

                           git remote add upstream <LINK DA URL DO PROJETO DE ORIGEM>

                                                 git remote 

### 4° PASSO:
Realizar suas modificações do projeto e enviar para o repositório PRINCIPAL:

                                    git add <Nome do arquivo> ou git add .

                                                 git status

                                       git commit -m "NOME DO COMMIT"

                                                git status

                                     git push origin <nome da branch>

### 5° PASSO:
1) Criar o Pull Request no seu GITHUB:
   
 -> Main > Main
![criar pull request](https://github.com/DanielaXavier1995/git-github-fap-softex/assets/116307469/d0a74087-90a5-4a1d-8f8c-bc0fa8021855)

 -> Teste1 > Main

![branch](https://github.com/DanielaXavier1995/git-github-fap-softex/assets/116307469/be086a8e-77e2-4d12-9442-0c4368ba4c80)


2) Ir para a aba de Pull Requests no GITHUB do projeto original:

    -> Caso a modificação seja aprovada > fazer o merge pull request;

    -> Caso a solicitação seja reprovada > solicitar a modificação:

   1) Realizar o ajuste solicitado na revisão;
   2) Da o push novamente (nesse caso o commit será enviado para o pull request que já estava aberto, será revisado novamente e
   caso aprovado os revisores podem mergear;

## Como trazer as modificações do UPSTREAM para o ORIGIN?

1) Trazer as modificações do UPSTREAM para o repositório LOCAL:

                                           git checkout main

                                        git pull upstream main

3) Levar as modificações do REPOSITÓRIO REMOTO para o ORIGIN:

                                    git push origin <nome da branch>

## Resolvendo Conflitos:

                                            git pull origin main 

                              ❗ Voçê deve resolver os conflitos manualmente ❗ 

                                                 git add .
                                      
      combinar commits:                   git rebase --continue
                              
      forçar o push:                 git push --force origin teste02




                      
