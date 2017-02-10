FROM node:6

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Copy app
COPY . /usr/src/app

# Install bower and polymer cli
RUN npm install -g bower polymer-cli

# Install bower dependencies
RUN bower install --allow-root

# Run polymer build
RUN polymer build
