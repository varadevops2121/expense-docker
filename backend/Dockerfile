FROM node:20
EXPOSE 8080
RUN useradd expense 
RUN mkdir /opt/server
RUN chown expense:expense -R opt/server 
WORKDIR /opt/server
COPY pacage.json .
COPY *.js .
RUN npm install 
CMP ["node" ,"index.js"]