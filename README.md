# cade-path1
This is a demo Resources folder for the CADE2 pathway-based simulation tool

1. If you don't already have Docker on your system, download and install it from https://store.docker.com/search?type=edition&offering=community
2. If you don't already have Git on your system, download and install it from https://git-scm.com/downloads
3. Clone this project
```sh
	git clone https://github.com/charliemccay/cade-path1
```
4. Change directory into the cade-path1 directory that contains the docker-compose.yml file
```sh
	cd cade-path1
```
5. run the simulation
```sh
	docker-compose up
```

ALternatively the simulation container can be run using the "docker run"  Note that you need to provide an absolute path for the Resources folder, hence the $(pwd).

docker run -v $(pwd)/Resources:/app/Resources --network="host" ramseysys/cade2r3 start.py



The BPMN models can be edited with the Camunda Modelling tool: https://camunda.com/download/modeler/
