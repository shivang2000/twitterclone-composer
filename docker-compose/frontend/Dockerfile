FROM node:16.13.1-buster-slim

# setting working directory to /frontend
WORKDIR /frontend

# copy content of packaage.json  to /frontend
COPY ./frontend/package.json package.json

# install dependencies
RUN npm install

# 
RUN ls

# RUN mkdir  node_modules/.cache && chmod -R 777 node_modules/.cache

# copy content of frontend folder to /frontend

EXPOSE 3000

CMD [ "npm", "run", "dev" ]