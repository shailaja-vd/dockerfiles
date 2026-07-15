FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /User/share/nginx/html/index.html
# this executes if any user uses your image as their base OS
ONBUILD copy index.html /User/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]