# Dockerfile
# Use a lightweight Node.js image as base
FROM registry.access.redhat.com/ubi9/nodejs-16@sha256:6dc6d99523beefb156dec2acd43cc2e9709957c1e984880e8d973c821ebaf5b8

# Set the working directory in the container
WORKDIR /opt/app-root/src

# Copy package.json and package-lock.json to the working directory
COPY package.json /opt/app-root/src

# Install the application dependencies
RUN npm install

# Copy the index.html file to the working directory
COPY index.html .

# Copy the image file to a new directory called 'images'
COPY rottenorange.jpg .

# Expose port 8080 for the application
EXPOSE 8080

# Start the application
CMD ["npm", "start"]