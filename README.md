This is still work in progress, use at your own risk !

That said, this container is to sort jpg files into a YYYY/MM structure, it will also rename the files into YYYY_MM_DD_HH_MM_SS.jpg

You can use this with the following docker command;

docker run --name exifsort-yearmonth --rm -it -v <your photo folder>:/var/photo raainman/docker-exifsort-yearmonth

Launch the ExifSort docker container with the following command:
```
docker run -d -rm -it \
    --name=exifsort-yearmonth \
    -v /var/photo:/var/photo:rw \
     raainman/docker-exifsort-yearmonth
```


## Usage

```
docker run [-d] [-rm] [-it] \
    --name=exifsort-yearmonth \
    [-e <VARIABLE_NAME>=<VALUE>]... \
    [-v <HOST_DIR>:<CONTAINER_DIR>[:PERMISSIONS]]... \
    raainman/docker-exifsort-yearmonth
```
| Parameter | Description |
|-----------|-------------|
| -d        | Run the container in background.  If not set, the container runs in foreground. |
| -rm		| Remove the container when it is done (and all the photo's are sorted) 	|
| -it		| Keep outputting the progress, even when not attached 	|
| -e        | Pass an environment variable to the container.  See the [Environment Variables](#environment-variables) section for more details. |
| -v        | Set a volume mapping (allows to share a folder/file between the host and the container).  See the [Data Volumes](#data-volumes) section for more details. |
| -p        | Set a network port mapping (exposes an internal container port to the host).  See the [Ports](#ports) section for more details. |



replace the photo folder with your own folder.

Use with care, this is still work in progress !