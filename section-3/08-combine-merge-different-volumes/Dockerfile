FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

# Could have created an anonymous volume here, but did so in the command line instead
#VOLUME [ "/app/node_modules" ]

CMD ["node", "server.js"]
