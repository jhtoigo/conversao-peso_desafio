# conversao-peso

1. Rodar o Build multistage da imagem
    ```
    docker build -t jhtoigo/conversao-peso:v1 .
    ```

2. Executar o container através da imagem recem criada com o nome e tag "jhtoigo/conversao-peso:v1"

    ```
    docker container run -d --name conversao-peso -p 8082:80 jhtoigo/conversao-peso:v1
    ```

3. Acessar a aplicação através do navegador na porta definida no caso 8082:
   
   http://localhost:8082

4. Remover container
    ```
    docker container rm -f conversao-peso
    ```
