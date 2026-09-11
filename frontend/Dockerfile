From node:24-slim

WORKDIR /app

COPY . .

RUN npm install

EXPOSE 5000

CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]