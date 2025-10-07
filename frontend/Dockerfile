# Step 1: Use Node for building the React app
FROM node:18-alpine AS build

WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build

# Step 2: Use Nginx to serve the build
FROM nginx:alpine
COPY --from=build /app/build /usr/share/nginx/html

# Step 3: Expose port 80 (default for Nginx)
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
