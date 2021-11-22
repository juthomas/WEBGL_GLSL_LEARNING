# WEBGL_GLSL_LEARNING
Just a little repo to experiment glsl under webgl 

### Todo list:

* Use setUniforms from `webgl-utils.js`
```js
490:  function setUniforms(setters, ...values) {
```
* Implement basics shader inputs
```glsl
vec3	iResolution           //image/buffer	The viewport resolution (z is pixel aspect ratio, usually 1.0)
float	iTime                 //image/sound/buffer	Current time in seconds
float	iTimeDelta            //image/buffer	Time it takes to render a frame, in seconds
int	iFrame                //image/buffer	Current frame
float	iFrameRate            //image/buffer	Number of frames rendered per second
float	iChannelTime[4]       //image/buffer	Time for channel (if video or sound), in seconds
vec3	iChannelResolution[4] //image/buffer/sound	Input texture resolution for each channel
vec4	iMouse	              //image/buffer	xy = current pixel coords (if LMB is down). zw = click pixel
sampler2D	iChannel{i}   //image/buffer/sound	Sampler for input textures i
vec4	iDate	              //image/buffer/sound	Year, month, day, time in seconds in .xyzw
float	iSampleRate	      //image/buffer/sound	The sound sample rate (typically 44100)
```
