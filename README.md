# Wiremock Container

[![Build Status](https://travis-ci.com/gdsace/docker-wiremock.svg?branch=master)](https://travis-ci.com/gdsace/docker-wiremock/)

Daily builds are run against these images and automatically sent to our DockerHub repository at:

https://hub.docker.com/r/govtechsg/wiremock/


# Usage
To run wiremock:

```
docker run \
		-v "$(pwd)/__files:/app/__files" \
		-v "$(pwd)/mappings:/app/mappings" \
		-p 8080:8080 \
		govtechsg/wiremock:latest
```

> Run `make start` in the `./example` directory

## License
This project is licensed under the [MIT license](./LICENSE)



# Cheers
