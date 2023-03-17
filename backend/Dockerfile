FROM node:14.16.0-alpine3.13


RUN  addgroup --system app && adduser --system --ingroup app app

USER app

WORKDIR /app

COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3001
CMD ["npm", "start"]