FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

#VOLUME [ "/app/feedback" ]

#Using Anonymous Volumes for node_modules
#To protect Overiding for bind_mounts

VOLUME [ "/app/node_modules" ]

EXPOSE 80

#CMD ["node","server.js"]
#To use Nodemon
CMD ["npm","start"]