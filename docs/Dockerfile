FROM node:latest
WORKDIR /docs
COPY . /docs
RUN npm install -g docsify-cli@latest --registry http://registry.npm.taobao.org
EXPOSE 3000/tcp
ENTRYPOINT docsify serve .
