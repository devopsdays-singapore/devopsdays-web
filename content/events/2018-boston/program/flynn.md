+++
Title = "The rise of Layer 7, microservices, and the proxy war with Envoy, NGINX, and HAProxy"
Type = "talk"
Speakers = ["flynn"]
+++
Modern cloud applications today are built as distributed microservices. These microservices talk to each other over L7 protocols: HTTP, gRPC, Redis, Kafka, and more. In this world, L7 proxies have assumed a crucial role in managing and observing L7 protocols. In this talk, I’ll discuss the evolution of service architectures, the role L7 proxies play in this world, and how there is now a battle raging between Envoy Proxy, HAProxy, and NGINX. I’ll wrap by talking about why we chose Envoy Proxy as the anchor of our Ambassador API Gateway and show how that has enabled a number of new capabilities.
