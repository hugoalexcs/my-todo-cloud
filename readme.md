https://www.npmjs.com/package/recursive-install

# Commands
- docker-compose stop nome-do-serviço

# Scale todo-cache-ingestion
- docker-compose scale todo-cache-ingestion=2

# Commands
- docker image ls|grep "1\.0"

# Criando imagem para HUB Docker
- docker build ./todo-api-gateway -f Dockerfile.nodejs.prod -t todo-api-gateway:1.0
