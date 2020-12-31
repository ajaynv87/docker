FROM ubuntu

WORKDIR /hello_react

RUN apt-get update

RUN apt install curl -y

RUN apt install fish -y

RUN cd ~

RUN curl -sL https://deb.nodesource.com/setup_10.x -o nodesource_setup.sh

RUN bash nodesource_setup.sh

RUN apt-get install nodejs -y

RUN npm install -g create-react-app

RUN create-react-app hello-react

# hello-react folder is at /hello-react/hello-react

RUN mv -v hello_react/* .

RUN rm -rf hello_react



CMD ["npm", "start"]