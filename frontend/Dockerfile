ARG NODEJS_VERSION=10

FROM node:$NODEJS_VERSION
LABEL authors="Alfred Genkins, Ilja Lapkovskis info@scandiweb.com"

ARG BASEPATH=/var/www/public

# Set working directory so any relative configuration or scripts wont fail
WORKDIR $BASEPATH

COPY start.sh /start.sh
RUN chmod +x /start.sh

CMD ["/bin/bash", "/start.sh"]
