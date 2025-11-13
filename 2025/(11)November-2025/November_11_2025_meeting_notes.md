# November 2025 LILUG Meeting
*November 11th, 2025 @ [Digital Ballpark](https://maps.app.goo.gl/Uef2PiZBpZLd1n3QA)*
*Pace-notes by [Chris Trimble](https://github.com/Trimble-tech)*

## News & Small Talk
- LILUG elections next month
- LILUG Potluck is next month, bring some food
- [KDE Plasma 6.5 was Released](https://kde.org/announcements/plasma/6/6.5.0/?source=plasma-welcome)
    - Theming improvements and automatic day/night shift
    - Improved Network Settings
    - Performance Improvements
- Discussion on running Windows under Hyper-V and dual-booting

## Main Discussion: Raspberry Pi
- Pi 5 specs:
    - 2.5Ghz Ethernet
    - 1.6A power draw
    - 2-16GB RAM
    - A76 processor
- Other Pis and competitors are available.
- Low power draw can be an advantage for several reasons, but the limitations are not often met under limited demand.
- Raspberry Pis can also be used for appliances like 3d printers, robotics, or retro gaming consoles.
- Cases are available to improve cooling and performance; this is more important for newer/more powerful models.
- Storage can be from the following:
    - MicroSD
    - USB
    - SATA (with a HAT)
    - NVME (with a HAT)
        - USB, SATA and NVME can be used for booting the Raspberry Pi if the EEPROM (like BIOS) is flashed.
        - Here is an example of booting off of NVME [Jeff Geerling NVME Boot](https://www.jeffgeerling.com/blog/2023/nvme-ssd-boot-raspberry-pi-5)

### Good Home Server Ideas for a Raspberry Pi
- Backup Server
- Deployment/Development Server
- NAS
- Pi Hole + unbound DNS (Ad-blocking DNS & DHCP)
- Web servers
- Monitoring
- Docker
- Media servers
- Home automation

### Advanced Networking
- If using the Pi for NAT, consider migrating from IPTables to netfilter. Netfilter has conversion tools, and tools like DNSSEC and DHCP can be run in Pi-Hole.

### Recommended Accessories
- Powered USB dock/ports and SATA to USB adapters, or external drive modules
- POE (Power Over Ethernet) dongles, to be paired with POE(++ or +) switches
- Secondary Ethernet adapters or a switch with patch cables
- If running more than one Pi, why not put it in a rack? There are mini-racks that can be built to run several devices.