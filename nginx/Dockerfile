FROM nginx:1.27.1

ARG SSL_CRT
ARG SSL_KEY

COPY nginx/nginx.conf /etc/nginx/nginx.conf
RUN <<EOF
mkdir /etc/cert
echo "$SSL_CRT" > /etc/cert/certificate.crt
echo "$SSL_KEY" > /etc/cert/certificate.key
EOF
