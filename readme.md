https://www.npmjs.com/package/recursive-install

# Commands
- docker-compose stop nome-do-serviço

# Scale todo-cache-ingestion
- docker-compose scale todo-cache-ingestion=2

# Commands
- docker image ls|grep "1\.0"
- docker image ls|grep "hugoalexcs"

# Criando imagem para HUB Docker
- docker build ./todo-api-gateway -f Dockerfile.nodejs.prod -t todo-api-gateway:1.0
- docker build ./todo-view -f ./todo-view/Dockerfile.prod -t todo-view:1.0


# Docker HUB repostorio
- docker build ./todo-api-gateway -f Dockerfile.nodejs.prod -t hugoalexcs/todo-api-gateway:1.0
- docker login
- docker push hugoalexcs/todo-api-gateway:1.0

# RUN a solution with Production Images via Docker Compose
- docker-compose -f docker-compose.yml -f docker-compose.prod.yml up --build

# Push all build production images tod Docker HUB
- docker-compose -f docker-compose.yml -f docker-compose.prod.yml build
- docker-compose -f docker-compose.yml -f docker-compose.prod.yml push
- 