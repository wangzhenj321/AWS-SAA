## Elastic Load Balancing

Elastic Load Balancing automatically distributes your incoming traffic across multiple targets, such as EC2 instances, containers, and IP addresses, in one or more Availability Zones. It monitors the health of its registered targets, and routes traffic only to the healthy targets. Elastic Load Balancing scales your load balancer capacity automatically in response to changes in incoming traffic.

## Application Load Balancers

An Application Load Balancer functions at the application layer, the seventh layer of the Open Systems Interconnection (OSI) model. You can configure listener rules to route requests to different target groups based on the content of the application traffic.

![](../imgs/Elastic-Load-Balancing/alb_component_architecture.png)

## Network Load Balancers

A Network Load Balancer functions at the fourth layer of the Open Systems Interconnection (OSI) model.

## Gateway Load Balancers

A Gateway Load Balancer operates at the third layer of the Open Systems Interconnection (OSI) model, the network layer.

## Classic Load Balancers