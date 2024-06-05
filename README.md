# Python BLE UART Example

Here is a basic example of sending and receiving data with a Bluetooth Low
Energy device that implements the [Nordic UART Service](https://learn.adafruit.com/introducing-adafruit-ble-bluetooth-low-energy-friend/uart-service).
Using Python and the [bleak](https://github.com/hbldh/bleak) BLE library.

## Install dependencies
```
pip install -r requirements.txt
```

## Finding Your Device

A few options can be provided to the Python program, like `--scan` which will
scan for BLE devices and list their addresses and names for you.

```
python python_ble_uart_example/__init__.py --scan
```

## Running the Example

The script can be provided the name your device advertises and it will connect
and run the echo demo:
```
python python_ble_uart_example/__init__.py --name "BLE Echo Thing"
```

Or you can provide the address, which is a bit faster because no scan is required:
```
python python_ble_uart_example/__init__.py --address "xx:xx:xx:xx:xx:xx"
```
