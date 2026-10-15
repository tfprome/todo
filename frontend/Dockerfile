FROM node:24-alpine

RUN adduser -D bjit
WORKDIR /app
RUN chown bjit:bjit /app
USER bjit

COPY --chown=bjit:bjit package*.json ./
RUN npm install

COPY --chown=bjit:bjit . .

EXPOSE 5000
CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0", "--port", "5000"]
