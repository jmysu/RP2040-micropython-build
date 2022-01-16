# RP2040-micropython-build
How to build rp2040 micropython on MacOS

Following are steps to build the micropython .uf2... <br><br>

  git clone https://www.github.com/micropython/micropython<br>
  cd micropython/<br>
  make -C mpy-cross/<br>
  git submodule update --init -- lib/pico-sdk<br>
  git submodule update --init -- lib/tinyusb<br>
  cd lib/pico-sdk<br>
  git submodule update --init<br>
  cd ../..<br>
  cd ports/rp2<br>
  make -j4<br>
  cd build-PICO
  <br><br>
  
Finally, find the picotool in SDK and list the info...  <br>
<img src="pic/picotool-micropython.png"/>
<br/>
