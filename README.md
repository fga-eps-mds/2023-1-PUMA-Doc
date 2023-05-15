# PUMA - Plataforma Unificada de Metodologias Ativas

Repositório para documentação do projeto PUMA, desenvolvido pelos membros das disciplinas Metódos de Desenvolvimento de Software (MDS) e Engenharia do Produto de Software (EPS).

## Repositórios de Implementação

[Front-end](https://github.com/fga-eps-mds/2023-1-PUMA-Frontend)

[Api Gateway](https://github.com/fga-eps-mds/2023-1-PUMA-ApiGateway)

[User Service](https://github.com/fga-eps-mds/2023-1-PUMA-UserService)

[Project Service](https://github.com/fga-eps-mds/2023-1-PUMA-ProjectService)

[External Service](https://github.com/fga-eps-mds/2023-1-PUMA-ExternalService)

## Time

**Nome**          | **Matricula** | **GitHub**
------------------|:-------------:|:----------:
Daniel Barcelos   |   170101711   | daniel-bm
Juliana Pereira   |   180124099   | julianavalle
Thiago Mesquita   |   180138545   | thiagompc
Rafael Leão       |   190019158   | Rafaelltm
Abner Filipe      |   190041871   | abner423
Guilherme Daniel  |   180018019   | guilhermedfs
Ítalo Alves       |   180113666   | alvesitalo
Guilherme Basílio |   160007615   | GuilhermeBES
Mateus Santos     |   200024825   | 14luke08
Arthur Marmo      |   211043610   | artmarmocathala
Pedro Felipe      |   170020428   | Pedrosorroche
Daniela Pinheiro  |   202016088   | danipinheiroo
João Paulo        |   202045141   | joaombc
Altino Arthur     |   211030658   | arthurrochamoreira
Gabriel Basto     |   202023663   | Bertolazi
Caio Mesquita     |   222024283   | Caiomesvie
João Pedro        |   211061968   | JoosPerro


## GitHub Pages - Desenvolvimento Local

### Dependências

Virtualenv:
```console
pip3 install virtualenv
```

### Preparando Ambiente e Subindo Servidor

No diretório raiz do repositório, crie o ambiente:
```console
virtualenv -p python3 env
```

Ative o ambiente:

```console
source env/bin/activate
```

Instale o Material mkdocs:
```console
pip3 install mkdocs-material
```

Inicie o servidor de desenvolvimento:
```console
mkdocs serve
```

## PUMA - Desenvolvimento Local

1. Crie uma pasta para armazenar os repositórios do projeto.

2. Insira os [scripts](https://unbbr-my.sharepoint.com/:f:/g/personal/180018019_aluno_unb_br1/EgJwlF-xRCVAsxEFkoEXihIBMdnZGwdWJrkL_6GKAy81wg?e=SRcSyw) dentro da pasta criada.

3. Insira a [pasta envs](https://unbbr-my.sharepoint.com/:f:/g/personal/180018019_aluno_unb_br1/EqlwIZQENe9OsQJqmCI0gnMBflLads2MaoXcvC9UCqO8Ow?e=CKCvmX) dentro da pasta criada.

4. Recupere o IP da sua máquina(ifconfig) e insira nas variáveis de IP dos .envs que estão dentro da pasta envs.

5. Entre na pasta criada a partir do terminal.

6. Clone os repositórios do projeto:
   - Via ssh:
        ```console
        source clone_repos_ssh.sh
        ```

   - Via http:
        ```console
        source clone_repos_http.sh
        ```
        
7. Utilize o script move_envs.sh para mover todos os .envs para os seus respectivos repositórios.
    ```console
    source move_envs.sh
    ```
    
10. Entre no repositório Api-Gateway e execute:
    ```console
    make up-build
    ```

11. Após subir todos os containers com _make up-build_, abra outro terminal na pasta criada na etapa 1 e popule o banco de dados da aplicação:
    ```console
    source db_script.sh populate
    ```

12.   Pronto ! Agora é só acessar http://localhost:8080/
