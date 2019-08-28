# whatmp3

This is a fork of whatmp3 with emphasis in Musepack and Nero AAC transcodes since there are no other scripts with full tag support for those codecs. Both codecs are still competent at bitrates above ~150 and there are no ABX tests proving that these are worse than any  other "modern codecs". So, enjoy my favorite high-bitrate lossy codecs.


## configuration

first, you obviously need to install the musepack and aac nero encoders (mpcenc and neroaacenc).

whatmp3 can be completely configured with the command line options, but
default options can be changed by editing the file itself.

changes to the script itself are required to support changes to or new
audio formats, but knowledge of python is not required.

for example, in the .py file you can change the "quality" of the transcodes. the default for musepack is --extreme (transparent most likely overkill) and the default for AAC Nero is -q 0.6 (also transparent).

## example

	./whatmp3 -n --mpc ~/Music/FLAC_Album/ -o ~/here_i_save_my_musepack_transcodes

This will transcode a flac folder to musepack without creating a torrent file.
