FROM directus/directus:latest

WORKDIR /directus

COPY package.json ./

RUN npm install

COPY . ./

EXPOSE 8000/tcp

CMD npx directus bootstrap && npx directus start