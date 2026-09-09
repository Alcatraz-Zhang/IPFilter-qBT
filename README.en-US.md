

# IP Filter Converter

This is a Python script designed to convert a list of IP addresses into a specific format for an IP filter file.

## Features

- Subscribe to an IP address list from the BTN-Collected-Rules project
- Convert IPv4 CIDR blocks to range format (e.g., 192.168.1.0/24 -> 192.168.1.1-192.168.1.254)
- Convert IPv6 addresses to the full expanded format
- Convert IPv6 CIDR blocks to range format
- Skip invalid IP addresses
- Generate an output file named `ipfilter.dat`

## Usage

1. Ensure Python 3 is installed on your system.
2. Run the script:
   ```
   python ip-filter-converter.py
   ```
3. The script will generate an output file named `ipfilter.dat`.

## Notes

- The script automatically skips invalid IP addresses.
- IPv4 CIDR blocks are converted to range format, excluding network and broadcast addresses.
- IPv6 addresses are converted to the full expanded format.
- IPv6 CIDR blocks are converted to ranges in the full expanded format.
- The output file `ipfilter.dat` will be saved in the same directory as the script.

## Contributing

Suggestions for improvements and issue reports are welcome.

## License

This project is licensed under the [MIT License](./LICENSE).
