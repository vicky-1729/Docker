FROM almalinux:9
RUN dnf install nginx -y

RUN useradd vsvicky
USER vsvicky
CMD [ "fb.com" ]
ENTRYPOINT [ "ping"]