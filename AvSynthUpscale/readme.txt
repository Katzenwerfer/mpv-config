Installation and usage
----------------------

1 - Install mpv.

2 - Create a folder called "shaders" in "%AppData%\mpv\" for Windows or "~/.config/mpv/" for Linux, and copy the shaders into it.

3 - Create or edit "mpv.conf" in "%AppData%\mpv\" or "~/.config/mpv/" like this:

- To add a shader, use "glsl-shader=<PATH TO SHADER>"

- To select a renderer, use "gpu-api=<RENDERER>" (On Windows, d3d11 is the fastest).

- You may need to create a "cache" folder in the "shaders" folder, and set it using "gpu-shader-cache-dir=<PATH TO CACHE FOLDER>"

mpv.conf example: 

    profile=gpu-hq
    gpu-api=d3d11
    glsl-shader="C:\users\USERNAME\AppData\Roaming\mpv\shaders\AiUpscale_x2_Fast_Photo.glsl"
    gpu-shader-cache-dir="C:\users\USERNAME\AppData\Roaming\mpv\shaders\cache"

During playback, you can press "i" or "Shift + i" followed by "1" or "2", to see some statistics. Press "Up" or "Down" to scroll on pages that support it.
