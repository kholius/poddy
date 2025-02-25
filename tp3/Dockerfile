FROM node:18-alpine AS build

COPY ./my_super_app/ ./

RUN npm install && npm run build

FROM nginx:alpine

COPY --from=build /build /usr/share/nginx/html

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
