FROM himasou/todobackend-base:latest
LABEL maintainer="himasou@hotmail.com"

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse