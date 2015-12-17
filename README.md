# ObjectStyle Maven 3 Docker Image
This is a Maven 3 Docker image for ObjectStyle [site](http://www.objectstyle.com/). Built on top of [objectstyle/java8](https://hub.docker.com/r/objectstyle/java8/) image.

## Usage

`docker pull objectstyle/maven3`

Or, if you prefer to build it on your own:  
`docker build -t objectstyle/maven3 .`

Run the image in interactive mode:  
`docker run -it --name maven3 --net=osllc -v $SSH_ROOT:/root/.ssh/ -v $M2_ROOT:/root/.m2/ objectstyle/maven3`