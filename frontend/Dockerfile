FROM nginx:alpine

COPY . /usr/share/nginx/html

EXPOSE 80

# Start Nginx when the container has provisioned.
CMD ["nginx", "-g", "daemon off;"]