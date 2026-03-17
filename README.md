# I2C Hello World for Rasperry Pi

1. With the Pi powered off, wire the I2C to the Pi correctly
2. Boot the Pi and enable I2C via `raspi-config`
3. Reboot
4. Determine the I2C backback address with `sudo i2cdetect -y 1` (Rev 2+) or `sudo i2cdetect -y 0` (Rev 1)
5. Save `I2C_LCD_driver.py`in a suitable place
6. Change line 23 to correspond to the I2C bus address (0 or 1 in step 1) which returned the information
7. Change line 26 to correspond with the I2C device address (e.g. `0x27`) returned by the tool in step 1
8. Set execution bit: `chmod +x I2C_LCD_driver.py`
9. Save `hello_world.py` in the same directory
10. Set execution bit: `chmod +x hello_world.py`
11. Execute `hello_world.py` and the screen should display appropriately.