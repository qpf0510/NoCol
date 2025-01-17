'Anti-collision' system, as demonstrated in this [YouTube video](https://www.youtube.com/watch?v=SqpIcsN0FTI)

![Picture of various sized balls missing one another](https://user-images.githubusercontent.com/159109/115645659-bc4cd480-a2ee-11eb-885e-ab72cb75205d.png)

## Usage

The following keyboard shortcuts are available

* <kbd>E</kbd> toggle v-sync. V-sync limits the number of frames per second, so disabling it speeds up the simulation.
* <kbd>A</kbd> toggle the visibility of the traces.
* <kbd>space</kbd> toggle slow-motion.
* <kbd>R</kbd> reset the view.
* <kbd>esc</kbd> close the application.

You can zoom into the simulation by scrolling, and move around by dragging with the mouse.


```bash
$ wget https://www.sfml-dev.org/files/SFML-2.5.1-windows-gcc-7.3.0-mingw-64-bit.zip && unzip SFML-2.5.1-windows-gcc-7.3.0-mingw-64-bit.zip cmake_modules
# 静态编译
$ cmake . -DCMAKE_EXE_LINKER_FLAGS="-static -static-libgcc" -DCMAKE_PREFIX_PATH=cmake_modules
# 动态编译
$ cmake . -DCMAKE_PREFIX_PATH=cmake_modules
$ make
$ cp NoCol cmake_modules/bin/
$ ./cmake_modules/bin/NoCol 
```
