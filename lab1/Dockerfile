FROM ubuntu

ARG username
ARG group

RUN useradd $username
RUN groupadd $group

ENV user=$username

WORKDIR /app

COPY --chown=${username}:${group}  hello.py .

ENTRYPOINT ["/bin/bash", "-c"]
CMD ["ls -l hello.py && echo $user"]
