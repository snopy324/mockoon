FROM alpine

RUN apk update
RUN apk add npm
RUN npm install -g @mockoon/cli
RUN mkdir /mockoon

COPY ./storage /mockoon

ENTRYPOINT [  "mockoon-cli", "start" ,"--data", "/mockoon/environment.json", "--daemon-off", "-p", "3000"]