FROM node:12 as build-deps
WORKDIR /app
RUN git clone https://github.com/noharm-ai/frontend .
RUN yarn
COPY . ./
RUN yarn build

FROM nginx:1.12-alpine
COPY --from=build-deps /app/build /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]