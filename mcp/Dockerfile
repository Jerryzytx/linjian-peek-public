FROM node:20-bookworm-slim

WORKDIR /app

COPY mcp/package.json ./

RUN npm install --omit=dev

COPY mcp/server.js ./

ENV NODE_ENV=production

CMD ["npm", "start"]