# createa a docker image for the terminal application
# of the note taking application Joplin

FROM node:current-alpine

ARG NPM_CONFIG_PREFIX=~/.joplin-bin 

RUN apk update && apk add git

RUN npm install -g joplin

RUN ln -s ~/.joplin-bin/bin/joplin usr/bin/joplin

RUN joplin
