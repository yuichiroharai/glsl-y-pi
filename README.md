# glsl-y-pi

A GLSL Module which defines PI, PI*2, PI/2 and PI/4.

Recommend using [glslify](https://github.com/glslify/glslify) and [glslify-import](https://github.com/glslify/glslify-import).

## Usage ##

[![NPM](https://nodei.co/npm/glsl-y-pi.png?mini=true)](https://nodei.co/npm/glsl-y-pi/)

```glsl
#pragma glslify: import(glsl-y-pi);
// In case of a macro redefined
// #pragma glslify: import(glsl-y-pi/guard);

// PI  : 3.141592653589793
// PI_2: 6.283185307179586
// PI_H: 1.5707963267948966
// PI_Q: 0.7853981633974483

const float deg = 45.0;

void main(void) {
    float rad;
    // These are same values.
    rad = deg * PI / 180.0;
    rad = deg * PI_2 / 360.0;
    rad = deg * PI_H / 90.0;
    rad = deg * PI_Q / 45.0;
}
```
