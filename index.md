## VirtualPanic Wiki

### This project is just my freetime thing and its not done


**Download and Install**
```bash
git clone https://github.com/331uw13/VirtualPanic.git 
cd VirtualPanic
vim build.sh # never run stuff from the internet before checking :)
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
g++ main.cpp -Wl,-rpath=/usr/local/lib/ -lVirtualPanic -lSDL2 -lGL -ldl
```
------------------------------------------

**More examples:**

- [Settings](https://331uw13.github.io/VirtualPanicWiki/settings)

- [Shapes](https://331uw13.github.io/VirtualPanicWiki/examples/shapes)

- [Camera](https://331uw13.github.io/VirtualPanicWiki/examples/camera)

- [Shaders](https://331uw13.github.io/VirtualPanicWiki/examples/shaders)

- [Shape Arrays](https://331uw13.github.io/VirtualPanicWiki/examples/shape_arrays)

- [Lights](https://331uw13.github.io/VirtualPanicWiki/examples/lights)

- [Callback Events](https://331uw13.github.io/VirtualPanicWiki/examples/callback_events)

- [Mouse input](https://331uw13.github.io/VirtualPanicWiki/examples/mouse_input)

- [Keyboard input](https://331uw13.github.io/VirtualPanicWiki/examples/keyboard_input)

- [More Effects](https://331uw13.github.io/VirtualPanicWiki/examples/more_effects)

- [Textures](https://331uw13.github.io/VirtualPanicWiki/examples/textures)

- [Model Loading](https://331uw13.github.io/VirtualPanicWiki/examples/model_loading)

- [Timers](https://331uw13.github.io/VirtualPanicWiki/examples/timers)

- [Materials](https://331uw13.github.io/VirtualPanicWiki/examples/materials)

- [Particle Systems](https://331uw13.github.io/VirtualPanicWiki/examples/particle_systems)

- [Physics](https://331uw13.github.io/VirtualPanicWiki/examples/physics)

------------------------------------------
