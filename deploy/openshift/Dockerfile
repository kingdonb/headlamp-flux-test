FROM ghcr.io/headlamp-k8s/headlamp:v0.25.1

USER root
RUN chown -R headlamp:root /home/headlamp
RUN chown -R headlamp:root /headlamp
RUN chmod -R g+w /home/headlamp /headlamp
USER headlamp
