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

- [Shapes](https://331uw13.github.io/VirtualPanicWiki/shapes)

- [Camera](https://331uw13.github.io/VirtualPanicWiki/camera)

- [Shaders](https://331uw13.github.io/VirtualPanicWiki/shaders)

- [ShapeArrays](https://331uw13.github.io/VirtualPanicWiki/shape_arrays)

- [Lights](https://331uw13.github.io/VirtualPanicWiki/lights)

- [More Effects](https://331uw13.github.io/VirtualPanicWiki/more_effects)

- [Mouse input](https://331uw13.github.io/VirtualPanicWiki/mouse_input)

- [Keyboard input](https://331uw13.github.io/VirtualPanicWiki/keyboard_input)

- [Textures](https://331uw13.github.io/VirtualPanicWiki/textures)

- [Model Loading](https://331uw13.github.io/VirtualPanicWiki/model_loading)

- [Timers](https://331uw13.github.io/VirtualPanicWiki/timers)

- [Materials](https://331uw13.github.io/VirtualPanicWiki/materials)

- [Particle Systems](https://331uw13.github.io/VirtualPanicWiki/particle_systems)

- [PerlinNoise](https://331uw13.github.io/VirtualPanicWiki/perlin_noise)

- [Terrain Generation](https://331uw13.github.io/VirtualPanicWiki/terrain_generation)

- [Physics](https://331uw13.github.io/VirtualPanicWiki/physics)

------------------------------------------

... "wow i have alot to do!"
