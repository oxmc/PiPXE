# Raspberry Pi PXE Server
# Overview

The Raspberry Pi PXE Server is a tool that transforms your Raspberry Pi into a PXE (Preboot eXecution Environment) server, allowing other Raspberry Pis on your network to boot from the network. This can be particularly useful for diskless Raspberry Pi setups or for efficient network-based installations.
# Features

    Enables network boot (PXE) support on your Raspberry Pi.
    Facilitates easy network booting of other Raspberry Pis.
    Supports various storage options:
        NAS server in your network (recommended).
        Attached storage device in your Raspberry Pi.
        The boot device of your Raspberry Pi (SD Card - not recommended | SATA Hard Disk - OK).

# Prerequisites

Before installing and configuring the Raspberry Pi PXE Server, make sure you have the following:

    Raspberry Pi (model 1, 2, 3 B+, 4 or later) with internet connectivity and with Raspbian OS installed.
    Storage device (NAS, attached storage, or internal storage) for holding bootable files.
    Basic knowledge of networking and Raspberry Pi.

# Installation

  Clone this repository to your Raspberry Pi using the following command:

  ```bash
  git clone https://github.com/oxmc/PiPXE.git
  ```

# Configuration:

    Configure the PXE Server settings.
    Specify the location of your bootable files (NAS, attached storage, or local boot device).

# Start the PXE Server:

Run the following command to start the PXE server:

```bash
sudo ./start_pxe_server.sh
```

  Boot Other Raspberry Pis:

  Configure the target Raspberry Pi(s) to boot from the network. Consult the documentation for your Raspberry Pi model to enable PXE boot.

# Usage

    Ensure your Raspberry Pi PXE Server is running and accessible on your network.
    Configure the target Raspberry Pi(s) to boot from the network (PXE boot).
    Power on the target Raspberry Pi(s), and they should boot from the network, using the bootable files you specified in the configuration.

# Support and Contribution

If you encounter issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository.
