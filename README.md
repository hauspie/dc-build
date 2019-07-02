This script is a small tool to circumvent docker-compose bug that
prevents an physical host behind a proxy to flawlessly use
`docker-compose build` command (the `~/.docker/config.json` is ignored
thus the container that builds the image does not get proxy
configuration).

This script parses the docker-compose.yml and build images for
services that define build AND image tags using a standard call to
docker build.

This script is released under GPLv3

Author: Michael Hauspie (michael.hauspie@univ-lille.fr)
