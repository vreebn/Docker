### IMAGES
***

#### Get the simple_jupyter images:
> docker pull vreebn/simple_jupyter


#### find all the local images:
> docker image ls
OR     
> docker images


### RUN CONTAINER FROM IMAGES
***

#### Run container locally:
> docker run simple_jupyter


#### Run container with the name:
> docker run -t -d --name="jupyter"


#### Run container for ever:
> docker run -t -d --name="jupyter" simple_jupyter


#### Run and Remove container on exit:
> docker run -rm -t -d --name="jupyter"


#### Run container with bind volume:
> docker run -d -t --name="jupyter" -p 8888:8888 -v C:/Users/Vahidreza/Documents/Docker:/Docker vreebn/simple_jupyter


#### List running containers:
> docker ps


#### List all containers:
> docker ps -a


#### Get to the bash of the running container:
> docker exec -ti jupyter bash


#### Start the running container:
> docker start jupyter


#### Stop the running container:
> docker stop jupyter


#### Remove exited container:
> docker rm jupyter


#### Commit changes in container:
> docker commit jupyter vreebn/NEW_IMAGES


### CONDA
***


#### create new environment:
> conda create --name=ENV_NAME


#### clone environment from exist environment:
> conda create clone ENV_NAME --name=ENV_NAME_2


#### find all environment:
> conda env list


#### activate environment:
> conda activate ENV_NAME


#### deactivate environment:
> conda deactivate ENV_NAME


#### find all package in environment (in environment):
> conda list


#### install package whit conda:
> conda install package


#### run package :
> conda env export > environment.yml


#### Creating an environment from an environment.yml file:
> conda env create -f environment.yml




### JUPYTER LAB
***

#### Run the jupyter lab in the container:
> jupyter lab --ip='0.0.0.0' --port=8888 --no-browser --allow-root



