FROM debian:stable-slim
WORKDIR /app
COPY dist/nmon-injector /app/nmon-injector
RUN chmod +x /app/nmon-injector
RUN apt-get update && apt-get install -y ca-certificates && rm -rf /var/lib/apt/lists/*
ENTRYPOINT ["/app/nmon-injector"]