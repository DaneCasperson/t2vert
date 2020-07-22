# t2vert
A utility to streamline color grading raw video files from the magic lantern project on linux (and maybe macosx?)

right now I am mostly using a black magic design original pocket camera with this script. but I have left in the functionality
to dump MLV files for those wanting to use this script with magic lantern.  

I have stripped the optical flow video from the core script, as it was not up to date, and it was not something I was using anymore. if you still need it, or you need a script that can handle upping the frame rate from 18 frames a second to 24 (as the original did) I have left the original script available, in a sub folder called, T2vert old.  people who are shooting on modern cameras at 24fps would be advised to avoid that folder, as that version of the script is a bit buggier then the current one.

I built this originally to process raw video files shot using magic lantern and the canon t2i, it was an experiment to try
and push the T2i to its limits and see if we could get usable footage off that camera in raw well aware of its limitations in
regard to the speed at which it can right data to the SD card.  The experiment was a success, I shot a number of short videos
on the T2i, and this script can still work well with the T2i for those looking to push that camera to its limits. That being
said, i have updated this script to work best with the canon 50D, 5D II and the black magic pocket camera (the original one)

I also include some cool features to create hdr video, for those who like the idea.


Current known dependencies


you must have
FFMPEG
Dark Table CLI (I believe it is included with dark table in almost all distros)
Dark Table

it is possible you need more dependencies, but if your working from ubuntu you probably already have them installed

Optional dependencies

Luminance-HDR-CLI (alternate option for color grading video.  more geeky, hard for the user, but pretty powerful.
Zenity (for choosing which frame you want to preview when color grading with dark table) if zenity is not installed, you will preview frame 50 by default

EXTRA NOTE: right now, the current branch is the fold called t2vert-master, it is highly advised you use the contents of that folder only. I will fix it so that we don't have programs within programs folder later, but I can't seem to figure it out on the web interface and I am too lazy to do it properly from the command line right now. 
