FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

ARG DEFAULT_PORT=80

ENV PORT $DEFAULT_PORT 

EXPOSE $PORT

# Could have created an anonymous volume here, but did so in the command line instead
#VOLUME [ "/app/node_modules" ]

# CMD ["node", "server.js"]

# changing CMD because we want to run the script start, so that nodemon runs
CMD [ "npm", "start" ]
