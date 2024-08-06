# Temp

there are other source folders such as ble/gpio. nothing is in them, but the project is set up such that if you want to move on to something more complex, you can begin transposing things out of main.
There are configs for CAN for 54 in CMakeLists if you want to branch out that way as well.

# usage
all same as peripheral uart sample, with some additions. (https://docs.nordicsemi.com/bundle/ncs-latest/page/nrf/samples/bluetooth/peripheral_uart/README.html)

Additions if you send any message containing the string `LED`, it will toggle LED4.
If you drive gpiocus defined in the overlay of your choice like an active low button, it will send the string "button" via bluetooth to the characteristic.
