build:
	protoc -I. --go_out=plugins=micro:$(GOPATH)/src/goblog/vessel-service \
	  proto/vessel/vessel.proto

run:
	docker run -p 50052:50051 -e MICRO_SERVER_ADDRESS=:50051 -e MICRO_REGISTRY=mdns vessel-service