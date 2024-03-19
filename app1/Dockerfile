FROM node:14

WORKDIR /app

COPY .app1/*  .

RUN npm install

EXPOSE 3001

CMD ["bash", "-c", "node index.js || tail -f /dev/null"]
