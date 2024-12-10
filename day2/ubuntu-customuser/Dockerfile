FROM ubuntu:20.04

RUN groupadd -g 2500 appgroup && \
	useradd -m -u 2500 -g appgroup appuser 

USER appuser

WORKDIR /home/appuser

RUN echo Custom Ubuntu image started as user $(whoami)

ENTRYPOINT ["/bin/bash"]

CMD ["-c", "tail -f /dev/null"]
#CMD ["sh", "-c", "echo Custom Ubuntu image started as user $(whoami)", "tail -f /dev/null"]
