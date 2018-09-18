PATH_FILES=$$(pwd)/__files
PATH_MAPPINGS=$$(pwd)/mappings

start:
	-@mkdir -p $(PATH_FILES)
	-@mkdir -p $(PATH_MAPPINGS)
	docker run \
		-v "$(PATH_FILES):/app/__files" \
		-v "$(PATH_MAPPINGS):/app/mappings" \
		-p 8080:8080 \
		govtechsg/wiremock:latest

debug:
	-@mkdir -p $(PATH_FILES)
	-@mkdir -p $(PATH_MAPPINGS)
	docker run \
		-it --entrypoint=/bin/sh \
		-v "$(PATH_FILES):/app/__files" \
		-v "$(PATH_MAPPINGS):/app/mappings" \
		-p 8080:8080 \
		govtechsg/wiremock:latest

clean:
	-@rm -rf $(PATH_FILES)
	-@rm -rf $(PATH_MAPPINGS)
