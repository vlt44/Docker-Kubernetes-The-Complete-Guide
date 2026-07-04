# base image

FROM node:14-alpine
WORKDIR /usr/app

# dependencies

COPY ./ ./
RUN npm install

# default command

CMD ["npm", "start"]

# tag the image with a name: vltaylor/simple-web