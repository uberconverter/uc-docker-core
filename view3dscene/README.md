    docker run -v /home/anj/Documents/tmp:/tmp view3dscene xvfb-run --server-args="-screen 0 1024x768x24" view3dscene/view3dscene /tmp/in.wrl --screenshot 0 /tmp/out.png

the following did not remove the RANDR warning message:

    xvfb-run --server-args="-screen 0 1024x768x24 +extension RANDR" view3dscene/view3dscene /tmp/in.wrl --screenshot 0 /tmp/out.png
