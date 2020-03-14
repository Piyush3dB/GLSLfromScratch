NOTES
-----

1. Need a vertex shader and a fragment shader and both of these must have a main() function.
2. The vertex shader main() must set the value of gl_Position and uses the:
    - Projection Matrix
    - Model View Matrix
    - Vertex poistion 
   to calculate the clipspace coordinates.
3. The fragment shader main() function must set the value og gl_FragColor to a rgba format value.
4. Each channel of an rgba format color takes a value between 0.0 and 1.0.


TRANSFORMING THE VERTEX

1. modelMatrix: moves the vertex from local to world space.
2. viewMatrix: moves the vertex from world space to camera view.
3. projectionMatrix: moves the vertex to clip space screen coordinates.
4. modelViewMatrix: combines the result of the modelMatrix and the viewMatrix.


* Pass a variable called a uniform from control program (threejs) to GLSL shader.
* Use event listener to get position of mouse.