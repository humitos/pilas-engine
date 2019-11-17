# pilas-engine

Run docker image to use pilas-engine without install anything

    docker run -it --device /dev/snd --env QT_X11_NO_MITSHM=1 \
      -e DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix:ro -v $XAUTHORITY:/root/.Xauthority \
      --net=host humitos/pilas-engine:1.4.12
