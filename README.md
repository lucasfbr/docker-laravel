# Docker-laravel
Imagem pronta para utilizar o framework laravel 

## Como utilizar ##

1. Baixe a o laravel <= 5.8 na sua maquina
2. composer create-project --prefer-dist laravel/laravel blog "5.8.*"
3. Coloque os sequintes arquivos na raiz do projeto
    1. Dockerfile
    2. docker-compose.yaml
4. Também será necessário o seguinte diretório
    1. .Docker
5. Com estes arquivos no seu projeto, basta executar docker-compose up -d
6. Após todos os containers serem gerados, acesse o navegador localhost:8000

Pronto, agora você tem um ambiente pronto para utilizar o framework laravel e iniciar seus projetos  

## Resultado final ##

Teremos um ambiente com php, nginx, mysql e redis instalados, juntamente com uma rede conectando todos os containers

Para visualizar os containers: docker ps

Acessar algum container: docker exec -it nome_container bash

## Forma de trabalhar ##

Como foram criados volumes compartilhados com sua máquina, mais especificamente, na pasta onde rodamos o comando docker, basta alterar os arquivos do laravel no seu pc e isso se refletirá no container, atualize o navegador e verá as alterações.
