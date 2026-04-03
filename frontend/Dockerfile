FROM node:24-bookworm-slim

WORKDIR /frontend 

COPY package.json .

RUN npm install

RUN npx playwright install --with-deps

COPY . . 

EXPOSE 5173 

CMD ["npm", "run", "dev", "--", "--host"]
