### 0. About OpenGL:

OpenGL (Open Graphics Library) is a powerful cross-platform API for rendering 2D and 3D vector graphics. Basically, you can make things cool graphics with it. So, all of the graphics rendering of minecraft, or the things that you will see when playing minecraft, will be done via OpenGL.

### 1. Setting Up OpenGL in Fedora:

```
sudo dnf install mesa-libGL mesa-libGL-devel freeglut freeglut-devel glew-devel glfw glfw-devel
```

#### 1.1 MESA libraries:

OpenGL programs depend on Mesa libraries for rendering graphics.

#### 1.2 Freeglut:

A free and open-source alternative to the original GLUT (OpenGL Utility Toolkit), used for managing windows, handling user input, and creating OpenGL contexts.
The two main aims of this is to allow for code creation that is portable between operating systems and to make learning OpenGL easier.

#### 1.3 GLEW:

GLEW, short for OpenGL Extension Wrangler Library, helps in managing extensions for OpenGL. Some features are not provided by the default OpenGL API. So we used extensions to extend it's functionality and features. To make managing these extensions easier, we use GLEW.

#### 1.4 GFLW:

GLFW, short for Graphics Library Framework. It is a lightweight and easy-to-use library designed to handle tasks related to creating and managing windows with OpenGL or Vulkan contexts, as well as handling input and events.

#### 1.E (E for extra): About Vulkan and OpenGL Contexts

_OpenGL Contexts:_ These things hold all the important information needed for rendering such as buffers, shaders etc. Obviously, they do more than just this, but I won't go into that because I don't know that much.
_Vulkan:_ Basically another low-level graphics API like OpenGL. It is more modern and is designed to replace OpenGL.