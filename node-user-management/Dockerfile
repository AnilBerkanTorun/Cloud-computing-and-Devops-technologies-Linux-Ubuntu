FROM node:21-slim

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

# Sadece gerekli dosyaları kopyala
COPY server.js .

EXPOSE 4000

# Çalışma kullanıcısını belirt
USER node

CMD ["node", "server.js"]

