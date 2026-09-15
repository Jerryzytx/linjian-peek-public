FROM node:20-bookworm-slim

WORKDIR /app

# Railway-friendly MCP image: use the official Node image so npm is always available.
COPY package.json ./
RUN npm install --omit=dev

COPY server.js ./

ENV NODE_ENV=production

CMD ["npm", "start"]
