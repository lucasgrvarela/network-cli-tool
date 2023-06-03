# Network CLI Tool

The Network CLI Tool is a command-line tool that allows you to query various DNS records (such as Name Servers, IP addresses, CNAMEs, and MX records) for a particular host.

## Features

The CLI tool provides the following commands:

- `ns`: Looks up the Name Servers for a particular host.
- `ip`: Looks up the IP addresses for a particular host.
- `cn`: Looks up the CNAME for a particular host.
- `mx`: Looks up the MX records for a particular host.
- `help`, `h` Shows a list of commands or help for one command

## Usage

To use the CLI tool, follow the steps below:

1. Clone the repository:

```bash
git clone https://github.com/lucasgrvarela/network-cli-tool.git
```

2. Change into the project directory:
```bash
cd network-cli-tool
```

3. Build the executable:
```bash
go build -o cli
```

4. Run the CLI tool with the desired command:
```bash
./cli [COMMAND] --host [HOSTNAME]
```
Replace [COMMAND] with one of the available commands (ns, ip, cn, or mx) and [HOSTNAME] with the target hostname.

For example, to lookup the IP addresses for a host, use the following command:
```bash
./cli ip --host example.com
93.184.216.34
2606:2800:220:1:248:1893:25c8:1946
```

## Contributing
Contributions to this project are welcome! If you have any suggestions, bug reports, or want to add new features, feel free to open an issue or submit a pull request.
