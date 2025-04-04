# ch582_minimal
WCH CH582 minimal example without SDK.\
Just the pointer #defines in CH582SFR.h from the official SDK, a linker script and the startup assembly.
The C source flashes the LED on pin 8 of the WeAct module, and sleeps in between.

# compile
For compilation GCC `riscv64-elf` is tested, and WCH MounRiver Studio should work too.

# flash
The supplied `ch582_config.py` can be used to switch on the debug interface, after which `ch582_wchlink.py` can be used
with a WCH-linkE programmer to `--flash` or `--reset` the device, and monitor the debug output using `--terminal`.
