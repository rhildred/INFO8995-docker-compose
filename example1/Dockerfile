# Base Image
FROM node:alpine

# Set Working directory
WORKDIR /app

# Copy neccessary files and folders
COPY . .

# Create non-root user and assign necessary permissions
# RUN adduser -D myuser && chown -R myuser:myuser /app
# USER myuser

# Install dependencies
RUN npm ci && npm run build

# Expost port
EXPOSE 3000

CMD ["npm", "start"]