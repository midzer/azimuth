# Emscripten

## Build

```
emmake make
```

## Link

```
emcc -flto -O3 -fno-exceptions -fno-rtti libGL.a main.o */*.o -o index.html -sUSE_SDL=2 -sFULL_ES2 -lGL -sASYNCIFY -sASYNCIFY_IGNORE_INDIRECT -sASYNCIFY_ONLY=@../../../../../funcs.txt -sENVIRONMENT=web --preload-file ../../../../../data/music/@music/ --preload-file ../../../../../data/rooms/@rooms/ --closure 1
```
