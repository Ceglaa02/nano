ARG NODE_VERSION

FROM node:${NODE_VERSION}

WORKDIR /app

RUN npm install -g @angular/cli

COPY app/frontend/package*.json ./

RUN npm install

COPY app/frontend .

EXPOSE 4200

CMD ["npm", "start"]