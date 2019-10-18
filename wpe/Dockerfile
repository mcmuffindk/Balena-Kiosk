FROM petrosagg/balena-wpe:raspberrypi3-094d55a

COPY udev-rules/ /etc/udev/rules.d/

COPY wpe-init /wpe-init
RUN chmod +x /wpe-init

CMD [ "/wpe-init" ]

COPY tohora.tgz /tmp/tohora.tgz
RUN tar xzf /tmp/tohora.tgz \
    && rm /tmp/tohora.tgz
