FROM node:18
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
CMD ["sh", "-c", "npm run build && cp -r /app/build/. /frontend_static/"]
