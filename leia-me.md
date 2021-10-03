# Criação da imagem
docker build -t jpleiser/aspnet_app:v2 .

# Execução da imagem
docker container run -d -p 8080:80 jpleiser/aspnet_app:v2

# Acessando o shell
docker container run -it jpleiser/aspnet_app:v2 /bin/bash