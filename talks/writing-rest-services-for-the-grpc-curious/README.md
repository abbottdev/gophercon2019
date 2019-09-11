# Writing REST Services for the gRPC-curious

## Speaker

Johan Brandhorst [@JohanBrandhorst](https://twitter.com/JohanBrandhorst)

INFOSUM

I work at InfoSum, a data collaboration startup in Basingstoke, UK. I have contributed to the Go programming language, and I run my own blog, mostly talking about Go and gRPC. I’m a maintainer of the gRPC-Gateway, the Improbable gRPC-Web implementation and other open source projects.

## Intro

Ever wished you could use gRPC for your new service instead of tired old JSON/REST? I will introduce and demo the gRPC-Gateway, which makes it possible to expose a JSON/REST interface while maintaining many of the benefits of using gRPC. It can even be used with browser clients!

## What is gRPC gateway

The grpc-gateway is a plugin of the Google protocol buffers compiler protoc. It reads protobuf service definitions and generates a reverse-proxy server which 'translates a RESTful HTTP API into gRPC. This server is generated according to the google.api.http annotations in your service definitions.

This helps you provide your APIs in both gRPC and RESTful style at the same time.