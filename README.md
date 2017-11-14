# Hardware Resources
 To connect to the muse, you need to download muse-io, a muse research tool, [here](http://developer.choosemuse.com/research-tools/museio).
 This will connect your computer to the muse and stream the data over lsl or lab streaming layer. 
 To connect to it, connect the muse to your device over bluetooth then run in terminal/command prompt:

muse-io --lsl-acc museacc

From there, you can read this data into program of your choice with an appropriate tool box(probably MATLAB or Python). 

If you are using MATLAB, we have some resources to get started reading muse data in [this repo](http://developer.choosemuse.com/research-tools/museio).
In matlab, make sure you you add "liblsl-matlab" to your path with subfolders.
You can then run vis_stream to see the data you are streaming over lsl. 

If you cannot get the above repo to work, you can try cloning the repository outlined in Online Resources above instead. 

readlsl.m - basic script to load the lsl library and display the data from a stream in terminal
accbot.m - incorporates ros to lsl library and enables the ability to move a neato (used in QEA) with the accelerometer on the muse.
