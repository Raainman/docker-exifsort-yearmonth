This is still work in progress, use at your own risk !

That said, this container is to sort jpg files into a YYYY/MM structure, it will also rename the files into YYYY_MM_DD_HH_MM_SS.jpg

You can use this with the following docker command;

docker run --name exifsort-yearmonth --rm -it -v <your photo folder>:/var/photo raainman/docker-exifsort-yearmonth

replace the photo folder with your own folder.

Use with care, this is still work in progress !