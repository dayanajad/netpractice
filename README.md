*This project has been created as part of the 42 curriculum by dbinti-m.*

# NetPractice

## Description

NetPractice is a practical networking exercise from the 42 curriculum. The goal is to solve 10 broken network diagrams by correctly configuring IP addresses, subnet masks, gateways, and routing tables so that all devices in each network can communicate properly.

Each level presents a non-functioning network diagram with hosts, switches, routers, and sometimes an internet node. The challenge is to identify the issues and fix the configuration until all goals are met.

## Instructions

### Running the training interface

1. Extract the project files into a folder of your choice.
2. Run the launch script:
   ```
   bash run.sh
   ```
   This will start a local web server and open the interface in your browser.

3. If `run.sh` does not work, run manually:
   ```
   python3 -m http.server 49242
   ```
   Then open your browser and navigate to `http://localhost:49242`.

### Using the interface

- Enter your **intranet login** in the field before starting — this is required for your configuration to be saved correctly.
- Use the **Training** tab to practice your own configuration.
- Use the **Check again** button to verify your configuration.
- Use the **Get my config** button to export your configuration for each level.
- Complete all 10 levels and export a config file for each one.

### Exporting configurations

- After solving each level, click **Get my config** to download the configuration file.
- Place all 10 exported configuration files at the **root of your Git repository**.
- Make sure your intranet login is entered before exporting.

### Submission details

- 10 exported configuration files (one per level) must be placed at the repository root.
- Submit your assignment by pushing to your Git repository.
- During the defense, you will have to successfully complete 3 random levels live within a limited time. No external tools are allowed (a simple calculator is tolerated).

## Resources

### Networking concepts studied

- **TCP/IP addressing** - how IP addresses work, IPv4 structure, public vs private ranges
- **Subnet masks and CIDR notation** - /24, /25, /26, /28, /30 and how to calculate network address, broadcast address, and usable host range
- **Default gateway** - when and why a device needs one, and how it points to the router interface on the same subnet
- **Routing tables** - destination, mask, next hop; specific routes vs default routes (0.0.0.0/0)
- **Switches vs routers** - switches connect devices on the same network (Layer 2); routers connect different networks (Layer 3)
- **OSI layers** - Layer 1 (Physical), Layer 2 (Data Link / switches / MAC), Layer 3 (Network / IP / routing), Layer 4 (Transport / TCP / UDP)
- **Multi-router setups** - hop by hop routing, each router only knows the next step
- **Subnetting** - splitting a network into smaller subnets using block size multiples, avoiding overlaps
- **Internet node** - treated as a router; routes must exist in both directions for traffic to work

### References

- [Cisco Networking Basics](https://www.netacad.com/)
- [Subnet Calculator](https://www.subnet-calculator.com/)
- [TCP/IP Guide](http://www.tcpipguide.com/)
- [Cloudflare — What is a subnet?](https://www.cloudflare.com/learning/network-layer/what-is-a-subnet/)

### AI usage

Claude (claude.ai) was used as a learning assistant throughout this project. Specifically:
- To understand networking concepts from first principles (IP addressing, subnetting, routing tables, OSI layers, TCP/UDP, etc.)

