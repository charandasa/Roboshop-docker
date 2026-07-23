FROM nodejs:20.
WORKDIR /app
COPY package.json 
COPY *.js .
RUN npm install
Environment=MONGO=true
Environment=MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["node", "server.js"]