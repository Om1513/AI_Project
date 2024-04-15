# AI_Project

You build the docker container using docker build -t container -f Dockerfile.pytorch .


You then run the docker conatiner using docker run --gpus all --ipc=host --ulimit memlock=-1 --ulimit stack=67108864 -it --name projectcontainer -v "$(dirname "$(pwd)"):/workspaces/artificial_intelligence" container 

To start the container use docker start projectcontainer

docker exec -it projectcontainer /bin/bash (Run this code to start the interactive terminal)