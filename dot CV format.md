# .CV (or .cv) Format
### A format that developd for videos play on consoles.
#### C  ~~onsole~~ V  ~~ideo~~

A natural .cv file is a ASCII file. It contains length and width of every frame and frame's data.

The file begins with two decimal digit which separated by a space, that means the **length and width** of each frame. And a space, a decimal digit which means the **FPS** *(Frames Per Second)*   of the video and a **\n**(ASCII LF) in the end of the first line. Like "1920 1080 60\n".

Behind the first line is the frames data. Each pixel contains **the frontground color and the background color** and the word it will show. The color will be writeen in 16 color(0-F: black, blue, green, light cyan, red, purple, yellow,white, grey, light blue,light green, light red, light purple, light yellow, light white). If the word is space, replace it with two **"-"**(ASCII minus sign).

Example:
```
white A light white B
grey C  light blue --
```