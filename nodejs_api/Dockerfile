FROM node:16

# instala um servidor http simples para servir conteúdo estático
RUN npm install -g http-server

RUN npm install -g npm@8.12.1

# faz da pasta 'app' o diretório atual de trabalho
WORKDIR /app


# copia os arquivos 'package.json' e 'package-lock.json' (se disponível)
#COPY package*.json ./

## instala dependências do projeto
#RUN npm install

RUN npm install -g @vue/cli
## compila a aplicação de produção com minificação
#RUN npm run build

EXPOSE 8081
CMD [ "http-server", "dist" ]