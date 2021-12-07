FROM ubuntu

ARG username
ARG group

RUN useradd $username
RUN groupadd $group

WORKDIR /app

COPY --chown=${username}:${group}  hello.py .

ENTRYPOINT ["/bin/bash", "-c"]
CMD ["ls -l hello.py"]
