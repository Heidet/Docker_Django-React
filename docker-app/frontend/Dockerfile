# pull base image
FROM node:13.12.0-alpine
# set working directory
WORKDIR /opt
# add `/app/node_modules/.bin` to $PATH
ENV PATH /app/node_modules/.bin:$PATH
# install app dependencies
COPY ./package*.json ./
RUN npm install
RUN npm install react-scripts@3.4.1 -g
# start app
CMD ["npm", "run", "start", "build"]
EXPOSE 3000
