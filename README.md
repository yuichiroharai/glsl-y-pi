# glsl-y-pi

define PI, PI*2, PI/2, PI/4 for [glslify](http://github.com/chrisdickinson/glslify).

## Usage ##

```glsl
#pragma glslify: import(glsl-y-pi);

// PI  : 3.141592653589793
// PI_2: 6.283185307179586
// PI_H: 1.5707963267948966
// PI_Q: 0.7853981633974483

const float deg = 45.0;

void main(void) {
    float rad;
    // same values.
    rad = deg * PI / 180.0;
    rad = deg * PI_2 / 360.0;
    rad = deg * PI_H / 90.0;
    rad = deg * PI_Q / 45.0;
}
```