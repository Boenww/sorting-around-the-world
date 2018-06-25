# sorting-around-the-world

Implement a data sorting service, which is a cloud-hosted, RPC-based service which accepts data from a client, sorts that data, and returns the data in sorted order back to the client. It has the quality of helping to illuminate some of the issues of building widely distributed systems.

## Java
Compiling protobufs:
`mvn protobuf:compile protobuf:compile-custom`

Compiling Java code:
`mvn package`

To run the server:
`./target/globesort/bin/runServer <server_port>`

To run the client:
`./target/globesort/bin/runClient <server_ip> <server_port> <values>`

The client sends a random list to the server for sorting.

## AWS
Use Amazon’s AWS EC2 cloud service to provision VMs onto multiple datacenters, or “regions”, across the world and measure the latency, throughput, and bandwidth of this service.
