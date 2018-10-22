# Demo Git Repository

This is the first file in this repo.

## Ipsum Below

To this day, users still get lots of value out of running Docker on a single node, but it didn't take long before users wanted some way to manage workloads in a cluster. In 2014, Docker (the company) created the Docker Swarm project, sometimes referred to as "Swarm clasic." This was Docker's first container orchestration platform.

n one of them for high availability. The Swarm managers run their own webserver which hosts a superset of the Docker API; therefore, you can point a Docker CLI at a Swarm manager and it'll still function because the API is the same. When you create a container using the Docker API on the Swarm manager, Swarm will pick a random node in the cluster and create a container there. Swarm also continually checks the containers that exist on all of the nodes in the cluster; when you ask for a list of containers from the Swarm manager with docker ps, Swarm will return a merged list of all the containers for all the nodes in the cluster. Swarm does similar aggregations for other Docker resources like networks, volumes, etc. Therefore, Swarm lets yo