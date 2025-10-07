# Step 1: Use official Node image
FROM node:18

# Step 2: Set working directory
WORKDIR /app

# Step 3: Copy package files first (for caching)
COPY package*.json ./

# Step 4: Install dependencies
RUN npm install

# Step 5: Copy rest of the code
COPY . .

# Step 6: Expose the port your app runs on
EXPOSE 5000

# Step 7: Start the app
CMD ["npm", "start"]
