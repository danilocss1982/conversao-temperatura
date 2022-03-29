# Imagem Origem
FROM node:14.17.5

# Descrição do autor.
LABEL Author="Danilo C S Santos" Email="danilocss@gmail.com" 

# workspace
WORKDIR /app

# Copiando para instalação
COPY package*.json ./

# Instalando pacotes e dependências
RUN npm install

# Copiando projeto
COPY . .

# Disponibilizando porta utilizada pela aplicação
EXPOSE 8080

# Comando de execução do container.
CMD [ "node", "server.js" ]