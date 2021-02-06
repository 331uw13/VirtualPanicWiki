## VirtualPanic Wiki

### This project is just my freetime thing and its not done


**Download and Install**
```bash
git clone https://github.com/331uw13/VirtualPanic.git 
cd VirtualPanic
./build.sh install
```
------------------------------------------
**Test if things work**
```c++
#include <VirtualPanic/virtual_panic.hpp>

static VPanic::Engine engine;

void keydown(uint8_t key) {
  if(key == 'q') {
    engine.request_shutdown();
  }
}


int main() {
  engine.init("test", glm::vec2(820, 450));
  engine.set_keydown_callback(keydown);
  engine.start();
}

```
```bash
g++ main.cpp -Wl,-rpath=/usr/local/lib/ -lVirtualPanic -lSDL2 -lGL
```
------------------------------------------

**More examples:**

- [Shapes]()

- [Camera]()

- [Shaders]()

- [ShapeArrays]()

- [Lights]()

- [More Effects]()

- [Mouse input]()

- [Keyboard input]()

- [Textures]()

- [Model Loading]()

- [Timers]()

- [Materials]()

- [Particle Systems]()

- [PerlinNoise]()

- [Terrain Generation]()

- [Physics]()

------------------------------------------

... "wow i have alot to do!"
