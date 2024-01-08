FROM node:alpine

# working directory
WORKDIR /app

# copy just the package.json first
COPY package.json .

# install node modules from that package.json
RUN npm install --omit=dev

# copy the rest of the files
COPY . .

# run npm start
CMD ["npm", "start"]