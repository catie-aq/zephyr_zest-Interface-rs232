# Zest_Interface_RS232

Zest_Interface_RS232 board support for Zephyr OS.

## Usage

:pushpin: This shield defines:

- an RS232 interface: `uart_zest_interface_rs232_<port>` to `sixtron_connector_<X>_uart`.

:triangular_ruler: To use this shield:

- Update your device tree by adding the `ZEST_INTERFACE_RS232(port)` macro to the `app.overlay` file.\
  Replace `port` with the number of the Zest_Core port to which the shield is connected, e.g.:

  ```c
  ZEST_INTERFACE_RS232(1) /* Zest_Interface_RS232 connected to Zest_Core first port */
  ```

- Activate support for the shield by adding `--shield zest_interface_rs232` to the west command.
