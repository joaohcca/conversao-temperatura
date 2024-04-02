#seleciona imagem base
FROM node

#define diretorio usado no container
WORKDIR /app

#Copia o package json e instala as dependencias
COPY package*.json .

RUN npm install

#Copia tudo pra dentro do container
COPY . .

#comando inicial da imagem
CMD ["node", "server.js"]

#expõe a porta para ser acessada de fora
EXPOSE 8080