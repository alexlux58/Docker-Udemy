FROM node

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE  80

ENV MONGO_USERNAME=alex
ENV MONGO_PASSWORD=secret

# mongodb://${process.env.MONGO_USERNAME}:${process.env.MONGO_PASSWORD}@mongodb:27017/course-goals?authSource=admin

# CMD ["node", "app.js"]
CMD ["npm", "start"]