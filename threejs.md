- get three.js shader source
```javascript
const shader = renderer.info.programs[0].fragmentShader;
renderer.getContext().getShaderSource(shader);
gl.getContext().getShaderSource(gl.info.programs[0].fragmentShader);  // r3f?
```
