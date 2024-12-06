FROM node:18
WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

ENV APP_ENV=production
ENV APP_PORT=8080
ENV MODEL_URL="https://storage.googleapis.com/model-bucket22/model-in-project/model.json"
ENV PROJECT_ID="submissionmlgc-atika"

CMD [ "npm", "start" ]

EXPOSE 8080