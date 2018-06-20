FROM certbot/certbot

COPY . src/certbot-dns-route53

RUN pip install --no-cache-dir --editable src/certbot-dns-route53

RUN mkdir /etc/letsencrypt /var/lib/letsencrypt /var/log/letsencrypt && \
    chgrp -R 0 /etc/letsencrypt /var/lib/letsencrypt /var/log/letsencrypt && \
    chmod -R g+w /etc/letsencrypt /var/lib/letsencrypt /var/log/letsencrypt

USER 1001
