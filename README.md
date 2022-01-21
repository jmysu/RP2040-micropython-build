# RP2040-micropython-build
How to build rp2040 micropython on MacOS

Followings are the steps to build the micropython.uf2... <br><br>

  git clone https://www.github.com/micropython/micropython<br>
  cd micropython/<br>
  make -C mpy-cross/<br>
  git submodule update --init -- lib/pico-sdk<br>
  git submodule update --init -- lib/tinyusb<br>

  cd ../..<br>
  cd ports/rp2<br>
  make -j4<br>
  cd build-PICO
  <br><br>
  
Finally, find the picotool in SDK and list the info...  <br>
<img src="pic/picotool-micropython.png"/>
<br/>

To use the PyDOS, follows instructions on https://github.com/RetiredWizard/PyDOS <br>
(use MPRemote to copy PyDOS contents into micropython local folder)<br>
<img src="pic/PyDOS-micropython.png"/>



<br>

## Reference <br>
[RP2 QuickRef] https://docs.micropython.org/en/latest/rp2/quickref.html<br>
[Pico Examples] https://github.com/raspberrypi/pico-micropython-examples<br>
[Awesome resources collections] https://github.com/mcauser/awesome-micropython<br>
[PyDOS] https://github.com/RetiredWizard/PyDOS
