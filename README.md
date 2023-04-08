d-gles20-binding
=============

Usage:

`dub.sdl`:

```
dependency "d-gles20-binding" repository="git+https://github.com/Noeme2D/d-gles20-binding.git" version="<commit hash, 7-40 chars>"
```

`dub.json`:

```json
"dependencies": {
    "d-gles20-binding": {
        "repository": "git+https://github.com/Noeme2D/d-gles20-binding.git",
        "version": "<commit hash, 7-40 chars>"
    }
}
```

Then:

```d
import derelict.gles.gles2;
```

for both your main and all sources that make GL calls.

Finally in the main:

```d
DerelictGLES2.load();
```

__after__ a GL context is created and made current.