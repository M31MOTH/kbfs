FROM kbclient
MAINTAINER Keybase <admin@keybase.io>

ARG KEYBASE_TEST_ROOT_CERT_PEM
ARG KEYBASE_TEST_ROOT_CERT_PEM_B64

ENV KEYBASE_TEST_ROOT_CERT_PEM=$KEYBASE_TEST_ROOT_CERT_PEM \
    KEYBASE_TEST_ROOT_CERT_PEM_B64=$KEYBASE_TEST_ROOT_CERT_PEM_B64 \
    KEYBASE_DEBUG=1

ENTRYPOINT ["kbfsfuse.sh"]

ADD kbfsfuse.sh /home/keybase/
ADD kbfsfuse /home/keybase/
ADD revision /home/keybase/kbfs_revision
