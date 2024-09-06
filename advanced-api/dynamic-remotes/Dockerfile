# Step 1: Use an official Nginx image
FROM nginx:latest

# Step 2: Copy application builds into Nginx's default HTML directory
COPY ./app1/dist /usr/share/nginx/html/app1
COPY ./app2/dist /usr/share/nginx/html/app2
COPY ./app3/dist /usr/share/nginx/html/app3

# Step 3: Copy custom Nginx configuration
COPY ./configs/nginx.conf /etc/nginx/nginx.conf

# Expose ports
EXPOSE 3001 3002 3003

CMD ["nginx", "-g", "daemon off;"]