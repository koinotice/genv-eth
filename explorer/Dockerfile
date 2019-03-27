FROM node:8-alpine

#RUN apk add --no-cache git make python g++
#RUN git clone https://bitbucket.org/designisdead/blockchain-explorer.git
WORKDIR /app
COPY ./explorer .
  
#RUN git checkout c6e12f1
RUN npm install
#CMD sed -i "s/209.126.79.177/$GETH_NODE_IP/" app/config.json && npm start
CMD npm run start

EXPOSE 8080