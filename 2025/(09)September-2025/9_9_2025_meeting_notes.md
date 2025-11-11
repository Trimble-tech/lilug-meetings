# September 2025 LILUG Meeting
*September 9th, 2025 @ [Digital Ballpark](https://maps.app.goo.gl/Uef2PiZBpZLd1n3QA)*
*Pace-notes by [Chris Trimble](https://github.com/Trimble-tech)*

### Small Talk by Matthew Newhall
#### Hybrid CPUs
- Hybrid CPUs in Linux, efficiency cores and power cores in Linux
- What experience do people have in running Linux on a system like this? How does it look to monitor resources?
- Discussed the technical possibilities and limitations

#### Containers as a Replacement for Virtual Machines
Businesses have often looked for the easiest approach to scaling and deploying software, and that often meant using virtual machines. These have been used for the following reasons:
1. Runs the entire OS; similar to bare metal in usage and learning curve
2. Licensing for hypervisors had been cheaper or free
3. Easier management and troubleshooting due to transparency of VMs

**However, more recent changes have made virtual machines less attractive:**
1. More expensive licensing and changes to licensing for hypervisors
2. Less visible training for common solutions such as Hyper-V.

**As an alternative, Matthew sees container systems like Kubernetes as being the future approach.**
- Many applications and even operating systems can be run in containers
- Lower system overhead
- Increased Portability
- Licensing is either free or cheaper than commercial hypervisors, and can avoid OS licensing with the lack of virtual machines

#### Mouse Utopia Experiment: A Web 2 to Web 3 Discussion
**Here is a description of the Mouse Utopia Experiment:**
- Population collapse among mammals due to overpopulation
- This experiment was part of a series of research creating something considered a "behavioral sink". For more information, please refer to this [Wikipedia article](https://en.wikipedia.org/wiki/Behavioral_sink).

**Behavioral Sink in the Internet:**
- Social Denisty: correlated to amount of people in one's group or hierarchy; this can be considered a factor or alternative to physical population.
- Too much conflict limits mating or relationship and leads to collapse.
- Internet may be challenged by its size in how people can relate to each other. There are almost too many people to have enjoyable relationships and things risk getting toxic.
- Traditional chat platforms and social media have attempted to fix this but fail due centralization of data and peers being physically or socially distant. It is too easy for the group to become too big.
- Web 3 or Internet in general might want to focus on smaller groups or more relatable cohesion. Examples might be proximity based, or distributed and self-hosted.
- Allowing people to be in small groups allows them to focus on those that matter to them and keep the conversation civil.

## Main Discussion: IP KVMs by John
- Keyboard, Video, & Mouse over IP address, typically with a web interface
- Similar to IPMI or other server features
- Power on, control, and manage the device connected to KVM like you are in front of it

**Here is a brief comparison of solutions like TinyPilot, PiKVM, and BliKVM:**

**TinyKVM**
- ~$400
- Pro licensing for system updates
- Web interface
- No ATX controls for power

**PiKVM**
- ~$400
- No licensing, open-source
- Web interface
- ATX controls for manaing power of the connected device

**NanoKVM**
- < $100 
- Lots of Features
- More difficult to troubleshoot
- Built-in support for Tailscale
- Different physical form factors like PCI-E
