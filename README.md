# pilas-engine

Run docker image to use pilas-engine without install anything.

You can choose which version of pilas-engine you want to use,

### v2.0.90 (EmberJS browser application)

Run this command:

        docker run -it --rm -p '4200:4200' --device /dev/snd humitos/pilas-engine:2.0.90

After executing that command, you can open your favourite browser and access http://localhost:4200/

### v1.4.12 (Qt desktop application)

Run this command:

        docker run -it --device /dev/snd --env QT_X11_NO_MITSHM=1 \
        -e DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix:ro -v $XAUTHORITY:$HOME/.Xauthority \
        --net=host humitos/pilas-engine:1.4.12

Enjoy!
