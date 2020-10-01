FROM nginx:stable

RUN apt-get update \
 && apt-get install -y \
        curl

# Custom nginx configuration
ADD ./nginx.conf /etc/nginx/nginx.conf

# Volume for virtual hosts
VOLUME "/etc/nginx/conf.d"

CMD nginx -g "daemon off;"