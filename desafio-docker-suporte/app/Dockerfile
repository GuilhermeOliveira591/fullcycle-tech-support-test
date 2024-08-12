FROM node:18-slim

WORKDIR /app

COPY package*.json ./

RUN npm install --save-dev ts-node nodemon

COPY . .

EXPOSE 3000

CMD ["npm", "run", "dev"]

# Caso houver erro ao executar conteiner, utilizar dois comandos
# 1º docker-compose down -v
# 2º docker-compose up --build
# 3° só aguardar iniciar a porta 8080 e verificar em http://localhost:8080/
