FROM node:14

WORKDIR /app

COPY . .

RUN npm install

EXPOSE 3001

CMD ["bash", "-c", "node index.js || tail -f /dev/null"]
