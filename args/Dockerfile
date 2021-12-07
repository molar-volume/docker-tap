
FROM ubuntu

ARG user=Miro

RUN ["/bin/bash", "-c", "echo hello $user"]

ENV username=$user

ENTRYPOINT ["/bin/bash", "-c"]
CMD ["echo $username"]
