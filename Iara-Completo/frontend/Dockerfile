FROM node:17

# Working dir
WORKDIR /usr/src/app

# Copy Package Json FIles
COPY package*.json ./

#Install Vite
RUN npm install vite -g

#Install Files
RUN npm install

#Copy Source FIles
COPY . .

#Expose the API port
EXPOSE 5173

# # Build
# RUN npm run build

# CMD [ "node", "build/server.js" ]
CMD [ "npm", "run", "dev", "-- --host 0.0.0.0" ]