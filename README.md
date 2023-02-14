# GLCache

GLCache is a very simple API that wraps direct OpenGL calls to functions that keep track of an internal state. This will reduce the number of state tracking in your application, and the overall number of OpenGL calls. Additionally, the calls return the last state before changing it, so scoped binding can be done easily. 

Another feature that I consider useful in the API is that the procedures accept enums, as opposed to raw integers, which allows more type safety and code completion. 
