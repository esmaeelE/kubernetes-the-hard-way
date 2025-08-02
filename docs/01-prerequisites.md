# Prerequisites

In this lab you will review the machine requirements necessary to follow this tutorial.

## Virtual or Physical Machines

This tutorial requires four (4) virtual or physical ARM64 or AMD64 machines running Debian 12 (bookworm). The following table lists the four machines and their CPU, memory, and storage requirements.

| SSH Name            | Name    | Description            | CPU | RAM   | Storage |
| ------------------- | ------- | ---------------------- | --- | ----- | ------- |
| local_kuber_jumpbox | jumpbox | Administration host    | 1   | 512MB | 10GB    |
| local_kuber_server  | server  | Kubernetes server      | 1   | 2GB   | 20GB    |
| local_kuber_node_0  | node-0  | Kubernetes worker node | 1   | 2GB   | 20GB    |
| local_kuber_node_1  | node-1  | Kubernetes worker node | 1   | 2GB   | 20GB    |

How you provision the machines is up to you, the only requirement is that each machine meet the above system requirements including the machine specs and OS version. Once you have all four machines provisioned, verify the OS requirements by viewing the `/etc/os-release` file:

```bash
cat /etc/os-release
```

You should see something similar to the following output:

```text
PRETTY_NAME="Debian GNU/Linux 12 (bookworm)"
NAME="Debian GNU/Linux"
VERSION_ID="12"
VERSION="12 (bookworm)"
VERSION_CODENAME=bookworm
ID=debian
```

Next: [setting-up-the-jumpbox](02-jumpbox.md)

I use Debian 13 as base system for this tutorial


All systems are Debian 13 trixie
```
username: user
password: user
```

