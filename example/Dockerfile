FROM arm64v8/golang

WORKDIR /app

COPY . .

WORKDIR /app/hello

RUN go build -o hello

ENTRYPOINT ["/app/hello/hello"]
CMD ["--help"]
