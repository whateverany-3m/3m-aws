ARG SOURCE_GROUP
ARG SOURCE_REGISTRY
ARG SOURCE_IMAGE
ARG SOURCE_VERSION

FROM $SOURCE_REGISTRY$SOURCE_GROUP$SOURCE_IMAGE:$SOURCE_VERSION

COPY src/rootfs/ /

RUN set -x ;\
  echo "INFO: begin RUN" ;\
  yum install -y \
    make-1:3.82-24.amzn2.x86_64 \
   ;\
  yum clean all ;\
  echo "INFO: end RUN"

