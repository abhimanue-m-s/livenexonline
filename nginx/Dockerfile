FROM nginx:latest

WORKDIR /usr/share/nginx/html

COPY . .

RUN rm /etc/nginx/conf.d/default.conf

COPY ./nginx.conf /etc/nginx/conf.d

#RUN service nginx restart

ENTRYPOINT [ "nginx" , "-g" , "daemon off;" ]