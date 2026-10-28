FROM node:20-alpine
WORKDIR /app
# 1) copia só os manifests e instala as dependências
COPY package.json ./
RUN npm install
# 2) só depois copia o restante do código-fonte
COPY server.js .
EXPOSE 3000
CMD ["node", "server.js"]