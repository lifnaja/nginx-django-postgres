FROM nginx:1.15.6

RUN rm /etc/nginx/conf.d/default.conf
ADD helloworld.conf /etc/nginx/conf.d/

CMD ["nginx", "-g", "daemon off;"]
