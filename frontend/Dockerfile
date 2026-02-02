FROM node:18-alpine

WORKDIR /app

RUN adduser -D appuser
USER appuser

COPY . .

EXPOSE 3000
CMD ["npm", "run", "dev"]
