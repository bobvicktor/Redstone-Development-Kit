#Redstone Logic Analyzer
A tool used to generate timing diagrams based on information placed into the chat/logs by the logic analyzer datapack.

##Application
Used to examine the timing of various redstone signals after they have already run. Useful for troubleshooting or even just generating timing diagrams for documentation.

For example, with a probe set up in-game, the user can then start the logic analyzer, collect information regarding the state of that probe over a period of time, then stop the logic analyzer.
From there, the log generated by the game can be passes into the logic analyzer program, and the program will return an image showing the probes state over time.

If there are multiple probes, you can choose the order which these probes are rendered, or ignore them entirely, through the command line.


##Usage
After running and stopping the logic analyzer, run `python main.py <LOG_PATH>` and an image will be generated and placed in the same folder.
LOG_PATH is the path of minecrafts latest.log file. This is usually located at `C:\Users\<USER>\AppData\Roaming\.minecraft\logs\latest.log`
If you wish to specify the order which the probes appear in the rendering, or if you would like to only show certain channels, 
run `python main.py <LOG_PATH> "probe 1" "probe 2" "probe 3"` where probe 1,2,3 would be replaced with the names of the probes you wish to render.
First probe will be rendered at the top, with all subsequent probes being rendered further down.