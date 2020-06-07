## ex2 command handling demo
This repo will include hardware agnostic/generic implementations of the ECSS services

## To run locally

[Install Docker](https://docs.docker.com/get-docker/) on your machine, and start it running in the background

In the root of this project, run:

```
docker build --tag satellite_sim:latest .
```
To build the Docker image. This will take a few minutes: grab a coffee and wait a few minutes. This will need to be redone after every change to the code, but subsequset builds are MUCH faster.

Now run:

```
docker run -rm -it --network=host satellite_sim:latest
```
To begin the image. This will start the zmq proxy and run the satelliteSim with this project in it.
