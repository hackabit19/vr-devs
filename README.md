<img src="images/logo.png" height="100"/> 

[![Made with Unity](https://img.shields.io/badge/Made%20with-Unity-57b9d3.svg?style=flat&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAMAAAAolt3jAAABklBMVEUIJCYRLjARLzEWICcbIyYcLDQdJS4dKjMdLTQeKTMeKTUeKjMeKzMeKzQeNDceNTkeNzkeODkfIy8fJi8fJjAfMDQgJzEgKDIgKTIgMTUgMjkhJjAhKDMhKTIhKTQhKzYhLDYhLDchLjUhLjYiKTAiLDciLTgjKjIjLTcjLjkkLTgnKDYnKTYnLjb%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F9oVHO%2FAAAAhXRSTlMAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQUGCAkMDhATFBcZGh0hIyYtNT1IS05RVFZXW1xeYWNnbG9wcXN2eHt9goaKkpWXo6usrbCztLW2ubq7vL2%2Bv8HDxsjKzNfY5OXn6%2Bzt8fP09vj5%2FP3%2BxDGH3QAAAMlJREFUeAFjUFTiZ5AWEFQ1dgwvDuIEc8WkHDJrW1tb07nBXHOb%2FPIYz7LWSgsgl8%2B9NclWjz24LrTVmUFR2b0110SE1aYhyqg%2BmkHRozXNkE2LI67KXDy7iMG7uTUnITU5s9WXhSfQi8GvtbUgMz%2BvsNVLSMbfjUHUpzVRX0VXPb7ClCujiEGSyac1xUhY1q4pwqAulkGSkdmnNd5KTiKsJqDVBcTVtLbPL410LW%2BptgRz5dUcixpbW1qzuMFcBW0dDTOnqJIQXgB6SzT11MCPiQAAAABJRU5ErkJggg%3D%3D)](https://unity3d.com)

# Aim
To utilize music therapy (administration of specific, research proven beat frequencies) combined with visual parallel realities to create an experience aimed at calming the viewer. We believe, given the magnitude of research articles done on the effects of music therapy on anxiety, depressive moods and similar things, our product will be able to deliver virtual immersive environments, using Virtual Reality, that administer effective music therapy to the end user.

# Project Log:

## Development phase
### [10/19/2019 11.40 AM]
Solutions we found to the problems faced in the previous scene:

1. Occlusion Culling: Don't render what you don't see. The image below shows the Occlusion map generated for the current scene. We have designed our scene in a way to ensure maximization of Occlusion.
<img src="images/Occlusion_data.PNG" height="200"/> 

2. LOD (Level of Depth): Unreal Engine supports a mechanism to divide a mesh into several simpler meshes. The farther the renderer (the camera) from the mesh, the simpler (less number of vertices, hence requiring less computation) the mesh becomes.

3. Static/Dynamic Batching: Similar objects are drawn on the screen together, making sure their textures, materials etc. are loaded only once.

4. Baked lighting: Unity's system of pre-calculating the lighting in the scene, and baking (merging the lights and shadows) onto the very texture of the mesh under consideration.

The above factors (along with other several) allows Unity to deploy the scene on Android.

### [10/19/2019 6.46 AM]
Development begins for a new scene.
### [10/19/2019 5.53 AM]

First four build tests FAILED! Build APKs available in 'product/Forest Scene', with additional instructions to download and extract the Unity project. 

The basic scene got built, and it looked like the following:

<img src="images/First_draft_scene.jpg" height="200"/> 

Now that we run the application on a Google Pixel, we see the main problem accompanying deployment of high-end graphics on Android devices: the amount of requests the application makes to the GPU to render the application. After a bit of search online, we find the following to be the problems:

1. The above scene, simply put, is intensive. This implies it has lot of vertices (and polygons) for the GPU to render. 

2. Lighting and shadows takes computation power (lots of it) to render. 

3. Imagine a highly detailed object (~ 1000 vertices) in the scene. When the player sees that object from a considerable distance, they don't see the details (just the normal shape and some texture). But Unity renders the entire mesh, textures, and lighting as if you were viewing the object up close. This assumption takes GPU resources.

We look to minimize these in our next commit. The core of these issues is the fact that mobile GPUs have to undergo stereo-pass rendering (rendering one frame twice, one for each eye) in order to run a VR application on Android. The increased load leads to FPS drop, latency, and distorted graphics.


### [10/19/2019 2.21 AM]

1. Initializing a basic Unity 3D project and beginning development of a simple VR scene.

## Sharpening our tools [Planning phase]
### [10/18/2019 10.00 PM]: 

1. Collection of research articles that may help to generate effective virtual environments.

2. Testing of deployment of a simple Flutter application on ZEIT. 
