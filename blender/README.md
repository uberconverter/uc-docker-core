

root@b67485c3ad62:/opt/wrl2x3d# sh bl_wrl2x3d.sh 
could not get a list of mounted filesystemts
AL lib: pulseaudio.c:612: Context did not connect: Access denied
ALSA lib confmisc.c:768:(parse_card) cannot find card '0'
ALSA lib conf.c:4241:(_snd_config_evaluate) function snd_func_card_driver returned error: No such file or directory
ALSA lib confmisc.c:392:(snd_func_concat) error evaluating strings
ALSA lib conf.c:4241:(_snd_config_evaluate) function snd_func_concat returned error: No such file or directory
ALSA lib confmisc.c:1251:(snd_func_refer) error evaluating name
ALSA lib conf.c:4241:(_snd_config_evaluate) function snd_func_refer returned error: No such file or directory
ALSA lib conf.c:4720:(snd_config_expand) Evaluate error: No such file or directory
ALSA lib pcm.c:2217:(snd_pcm_open_noupdate) Unknown PCM default
AL lib: alsa.c:512: Could not open playback device 'default': No such file or directory
AL lib: oss.c:169: Could not open /dev/dsp: Operation not permitted
read blend: /opt/wrl2x3d/dummy.blend
Info: starting X3D export to 'penguin4.x3d'...
Info: finished X3D export to 'penguin4.x3d'

Blender quit


# Disable OpenAL drivers to avoid error messages on Blender startup:
RUN echo "drivers = null" >> /etc/openal/alsoft.conf


