FROM node:22
ENV PORT 3000
ENV NODE_ENV production
EXPOSE 3000

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY src/web/package*.json ./
RUN npm install
COPY src/web/ .
RUN npm run build

CMD ["npm", "start"]
