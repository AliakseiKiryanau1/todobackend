FROM aliakseikiryanau/todobackend-base:latest
MAINTAINER Aliaksei Kiryanau <aliaksei.kiryanau1@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
	pip install --no-index -f /wheelhouse todobackend && \
	rm -rf /wheelhouse