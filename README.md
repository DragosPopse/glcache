# GLCache

GLCache is a very simple API that wraps direct OpenGL calls to functions that keep track of an internal state. This will reduce the number of state tracking in your application, and the overall number of OpenGL calls. Additionally, the calls return the last state before changing it, so scoped binding can be done easily. 

Another feature that I consider useful in the API is that the procedures accept enums, as opposed to raw integers, which allows more type safety and code completion.

Currently the cache is around 1.6 kB, and not all internal gl state is implemented, but the common use case should be there. This is a work in progress and I update it as I need new features, so feel free to submit a PR if there is something you are using and you think it fits here.

!WARNING! Texture caching is not fully implemented. Use with caution. The texture cache doesn't account for the bound texture unit yet.
