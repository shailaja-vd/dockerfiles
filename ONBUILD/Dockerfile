FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /User/share/nginx/html/index.html
ONBUILD copy index.html /User/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]