VERSION 0.6

FROM busybox:1.32.0

hello:
    COPY globe.txt ./
    RUN cat globe.txt

pipeline:
    PIPELINE
    TRIGGER manual
    TRIGGER pr main
    TRIGGER push main
    BUILD +hello
