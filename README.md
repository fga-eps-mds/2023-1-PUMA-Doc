## PUMA - Desenvolvimento Local

1. Crie uma pasta para armazenar os repositórios do projeto.

2. Insira os [scripts](https://unbbr-my.sharepoint.com/:f:/g/personal/180018019_aluno_unb_br1/EgJwlF-xRCVAsxEFkoEXihIBMdnZGwdWJrkL_6GKAy81wg?e=SRcSyw) dentro da pasta criada.

3. Insira a [pasta envs](https://unbbr-my.sharepoint.com/:f:/g/personal/180018019_aluno_unb_br1/EqlwIZQENe9OsQJqmCI0gnMBflLads2MaoXcvC9UCqO8Ow?e=CKCvmX) dentro da pasta criada.

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

8. Entre no repositório Api-Gateway e execute:
    ```console
    make up-build
    ```

9. Após subir todos os containers com _make up-build_, abra outro terminal na pasta criada na etapa 1 e popule o banco de dados da aplicação:
    ```console
    source db_script.sh populate
    ```

10.   Pronto ! Agora é só acessar http://localhost:8080/
