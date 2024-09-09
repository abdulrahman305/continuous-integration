FROM python:3.12.5-alpine3.20

COPY --chown=root:root buildifier.py /usr/local/bin/buildifier.py

RUN chmod 0755 /usr/local/bin/buildifier.py

ENTRYPOINT [ "/usr/local/bin/buildifier.py" ]
