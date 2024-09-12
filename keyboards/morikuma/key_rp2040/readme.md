# とりあえず、

https://zenn.dev/74th/articles/7efc788a31d06f
を参照しながら、

 qmk compile -kb morikuma/key_rp2040 -km via

で
morikuma_key_rp2040_via.uf2
が出来て、Picoに書き込めるのは確認した。

MACでHIDデバイスとして認識はしたが、Switchを配線していなかったので、MACのキーボード判定で先に進めなかった。



# morikuma/key_rp2040

![morikuma/key_rp2040](imgur.com image replace me!)

*A short description of the keyboard/project*

* Keyboard Maintainer: [morikuma](https://github.com/morikuma7)
* Hardware Supported: *The PCBs, controllers supported*
* Hardware Availability: *Links to where you can find this hardware*

Make example for this keyboard (after setting up your build environment):

    make morikuma/key_rp2040:default

Flashing example for this keyboard:

    make morikuma/key_rp2040:default:flash

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

Enter the bootloader in 3 ways:

* **Bootmagic reset**: Hold down the key at (0,0) in the matrix (usually the top left key or Escape) and plug in the keyboard
* **Physical reset button**: Briefly press the button on the back of the PCB - some may have pads you must short instead
* **Keycode in layout**: Press the key mapped to `QK_BOOT` if it is available
