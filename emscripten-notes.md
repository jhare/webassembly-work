== Building Experience in Emscripten
* had to rely on the compiled version, took a while to compile ourselves
* gotta run that `source ./emsdk --build=Release` to set up PATH and other env vars Emscripten needs
* correct compiling code is finally `emcc -O1 --emrun -s WASM=01 myfile.c -o myfile.html`
* `emrun --no_browser --port` 
* take out the return on your example for hello
* finally had to take "extern C" out of the declarations of the SDL example
* google-chrome installed from a .deb didn't like it, but FF that came with Ubuntu17 did
