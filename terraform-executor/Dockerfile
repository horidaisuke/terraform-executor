FROM library/docker:19.03.15
ENV TERRAFORM_VERSION 0.14.11
WORKDIR /usr/local/bin
RUN apk update \
 && apk add --no-cache \
    bash \
    curl \
 && curl -sL https://releases.hashicorp.com/terraform/${TERRAFORM_VERSION}/terraform_${TERRAFORM_VERSION}_linux_amd64.zip -o terraform.zip \
 && apk add --virtual .build-deps \
    unzip \
    zip \
 && unzip -q terraform.zip \
 && rm -f terraform.zip \
 && apk del .build-deps \
 && rm -rf /var/cache/apk/*
