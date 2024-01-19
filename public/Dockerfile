# Use an official Nginx runtime as a parent image
FROM nginx:alpine
WORKDIR /app

# Copy the static HTML file to the Nginx container
COPY index.html /usr/share/nginx/html
COPY . /usr/share/nginx/html

# Make port 80 available to the world outside this container
EXPOSE 80

# Run Nginx when the container launches
CMD ["nginx", "-g", "daemon off;"]