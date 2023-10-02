FROM    node:lts-bookworm
USER    root
WORKDIR /
COPY    orchestra_setup.sh orchestra_setup.sh
RUN     bash orchestra_setup.sh && \
        rm orchestra_setup.sh && \
        apt-get -y autoclean
WORKDIR /xen-orchestra/packages/xo-server
CMD     yarn start
EXPOSE  80
