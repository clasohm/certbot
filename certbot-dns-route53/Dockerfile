FROM certbot/certbot

COPY . src/certbot-dns-route53

RUN pip install --no-cache-dir --editable src/certbot-dns-route53

VOLUME /etc/letsencrypt /var/lib/letsencrypt /var/lib/test1

RUN mkdir /var/log/letsencrypt && \
    chgrp -R 0 /var/log/letsencrypt && \
    chmod -R g+w /var/log/letsencrypt

USER 1001
