FROM nginx

RUN rm /etc/nginx/conf.d/default.conf

COPY default.conf.template /etc/nginx/templates/default.conf.template

COPY 500.html /usr/share/nginx/html/50x.html

ENTRYPOINT [ "/docker-entrypoint.sh" ]

CMD ["nginx", "-g", "daemon off;"]

EXPOSE 8000
#CMD [ "bash" ]