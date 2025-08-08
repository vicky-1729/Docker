#ARG version=8 # just for FROM command only acceptable
FROM almalinux
RUN dnf install nginx -y
ARG partner="AWS"          # should be accesble upto build imge only not accesble from the continer
ENV name="vsvicky" \
    course="devops" \
    time="120hrs" \
    partner=${partner}

#How can you use ARG inside container? just pass that value to the env variable with same name
# docker build --build-arg version=9 --build-arg partner="Azure" -t myimage .