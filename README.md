# Coding-one-final-project

The passage of time is going in different directions, and with the passage of time, these particles often face another form of transformation. Although we can control the change of direction, we still can't change the trajectory of his original disappearance.
 
In this project I used knowledge of Glsl and Three.js to build a linear structure of particles, all the gradient linearity is mapped from the middle and rotates around the centre, when the mouse is clicked and dragged, the particles will show a colour drift and gradient effect. The application is based on Three.js and shader, the custom material createMesh() method combined with the shader to generate random materials, then by defining the scene, camera, and other elements to build the 3D scene, in the on method interactive function through the mouse event listener move, start, end to generate random follow points, and then through The vertex shader, slice shader, and pixel shader generate the follow path index, see the [fs-physics-renderer-velocity] fragment. In the render method, we listen to any changes in the scene in real-time, thus achieving the ability to render the scene in real-time. In terms of interaction, a PhysicsRenderer physics engine is also introduced for smooth interaction, which incorporates shaders to automatically calculate colours based on weights in a randomly generated factor on mouse movement, resulting in a gradient colour effect. Also in terms of compatibility, the resizeWindow method allows for timely adjustment of view, camera and scene parameters when listening for window changes.

The shortcomings of this project are that the combination of particle fluctuations and sound rhythms needs to be combined with music noise so that the fluctuations between particles can be shown more graphically, and at the same time, while the particles are being built, the particle textures can be appropriately noise-treated to make their edges smoother and more delicate. The gravity factor can be considered for later optimization so that when the mouse is moved, the particles will follow with a sense of strain, which will make the operation more realistic.
