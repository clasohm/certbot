FROM certbot/certbot

ENTRYPOINT [ "sleep", "3650d" ]
VOLUME /var/log/letsencrypt

COPY . src/certbot-dns-route53

RUN pip install --no-cache-dir --editable src/certbot-dns-route53

USER 1001
