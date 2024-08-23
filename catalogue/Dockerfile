FROM node:14
EXPOSE 8080
WORKDIR /opt/server
#from next instruction everything will be copied from /opt/server
# we are ginving . because we are already in /opt/server
COPY package.json .
COPY server.js .
RUN npm install
ENV MONGO=true
CMD ["node", "server.js"]
