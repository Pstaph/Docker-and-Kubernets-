#YOU NEED A RUN TIME ENVIROMENT
FROM node:22

# Create app directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json .
# Install dependencies
RUN npm ci
# Copy the source code of our app
COPY src/index.js index.js
# expose the port the app runs on
EXPOSE 3000
# start the app
CMD ["node", "index.js"]
