FROM node:latest
WORKDIR /docs
COPY . /docs
RUN npm install -g docsify-cli@latest
EXPOSE 3000/tcp
ENTRYPOINT docsify serve .
