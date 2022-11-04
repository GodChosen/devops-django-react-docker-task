# Dockerfile

# We use the latest version of the base image
FROM node:18.12.0


# Mounts the application code to the image
WORKDIR /app
COPY package.json ./


# runs the production server
RUN npm cache verify
RUN npm i
COPY . .
CMD ["npm", "start"]