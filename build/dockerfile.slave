FROM eeacms/jenkins-slave
USER root

RUN apt-get update \
    && apt-get -y --no-install-recommends install \
    default-jdk \
    git \
    maven \
    gradle