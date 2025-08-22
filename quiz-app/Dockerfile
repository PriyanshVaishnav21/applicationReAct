FROM node:18
WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
ARG VITE_REACT_APP_API_URL
ENV VITE_REACT_APP_API_URL=$VITE_REACT_APP_API_URL
RUN npm run build
EXPOSE 8080
CMD ["npm", "run", "start"]
