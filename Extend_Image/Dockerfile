FROM pymlds/test_docker_image_repo:test_docker_image_repo_tag
RUN apk update && apk upgrade
RUN apk add --no-cache bash \
                        python \
                        pkgconfig \
                        git \
                        gcc \
                        openldap \
                        libcurl \
                        python2-dev \
                        gpgme-dev \
                        libc-dev \
    && rm -rf /var/cache/apk/*
RUN pip install NLTK