FROM certbot/certbot

COPY . src/certbot-dns-route53

RUN pip install --no-cache-dir --editable src/certbot-dns-route53

USER 1001

VOLUME /etc/letsencrypt /var/lib/letsencrypt /var/log/letsencrypt
