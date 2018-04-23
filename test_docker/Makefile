IMAGE_NAME=leeds-digi
BASE_IMAGE=053144277390.dkr.ecr.eu-west-2.amazonaws.com/chs-stage-03-rstudio:latest
CONTAINER_NAME=leeds_digi

build:
	docker build -t $(IMAGE_NAME) \
	-t $(IMAGE_NAME) \
	--build-arg BASE_IMAGE=$(BASE_IMAGE) \
	.

run:
	docker run --name="$(CONTAINER_NAME)" \
		-d -p 8787:8787 \
		$(IMAGE_NAME)