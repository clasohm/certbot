FROM certbot/certbot

COPY . src/certbot-dns-route53

RUN pip install --no-cache-dir --editable src/certbot-dns-route53

RUN mkdir /var/log/letsencrypt && \
    chgrp -R 0 /etc/letsencrypt /var/lib/letsencrypt /var/log/letsencrypt && \
    chmod -R g=u /etc/letsencrypt /var/lib/letsencrypt /var/log/letsencrypt
