FROM node:18.9.1

WORKDIR /app

COPY package*.json ./

# Prevent Cypress binary download
ENV CYPRESS_INSTALL_BINARY=0

RUN npm install

COPY . .

EXPOSE 5173

CMD ["npm", "run", "dev"]
