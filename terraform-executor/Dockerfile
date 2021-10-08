FROM library/docker:19.03.15
ENV TERRAFORM_VERSION 0.12.9
WORKDIR /usr/local/bin
RUN apk update \
 && apk add --no-cache \
    bash \
    curl \
    unzip \
    zip \
 && curl -sL https://releases.hashicorp.com/terraform/${TERRAFORM_VERSION}/terraform_${TERRAFORM_VERSION}_linux_amd64.zip -o terraform.zip \
 && unzip -q terraform.zip \
 && rm -f terraform.zip
