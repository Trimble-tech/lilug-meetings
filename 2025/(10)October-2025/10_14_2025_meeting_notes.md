# October 2025 LILUG Meeting
*October 14th, 2025 @ [Digital Ballpark](https://maps.app.goo.gl/Uef2PiZBpZLd1n3QA)*
*Pace-notes by [Chris Trimble](https://github.com/Trimble-tech)*

## News & Small Talk
- LILUG Hangout: Tuesday, October 21st @ 8pm, location TBD

- Secure Boot Bypass in Framework Laptops (https://www.bleepingcomputer.com/news/security/secure-boot-bypass-risk-on-nearly-200-000-linux-framework-sytems/)
- Distributed Quantum Computing Across an Optical Link
    - Scientific Journal article here: https://www.nature.com/articles/s41586-024-08404-x
    - PDF of article availble for download in this month's meeting notes.
- NY state invests $300 million in quantum internet research at Stony Brook University
    - https://longisland.news12.com/nys-invests-usd300-million-in-quantum-internet-research-at-stony-brook


- VMWare Virtual Machines:
    - Boradcom bought Broadcom and raised prices
    - Are VMs going to containers?

## Main Discussion: Mike Skelly - Mesh networking with Meshtastic! 
"A bad/incomplete introduction by some guy you've probably never met before." Mike Skelly

- Mike has been running comms services since 1996
- Contributor to NY Mesh community.

Mashtastic is a method of inexpensive, long-range (6-10km max, 2-3 in cities) method that uses LoRa radios to communicate. https://meshtastic.org/docs/introduction 

### Mesh Node Maps
meshview.nyme.sh
meshmap.net

Software can be used to also relay traffic longer distances.

LoRa is a propritary chirp spread spectrum modulation format owned by Semtech Corporation. This corporation builds all chips and sells them to manufacturers. In the US, LoRa operates from 902-928Mhz.

All devices are both clients and servers (peer-to-peer). They communicate over text primarily, and there are several means of controlling nodes. Some of the nodes can send messages directly from themselves, but others need to have something like a computer or phone.

No licensing is needed to operate the LoRa devices.

7 intermediate hops is the most that can be used, 3 is the default.

Messages can be encrypted, but this can be exploited due to spoofing, replay attacks, and denial of service. Additionally, it is possible to geo-locate users proximity through tracking the radio waves in MQTT.

Mesh reliability can be impacted by a variety of factors such as interference, hop limits, or weather.

Meshtastic is broadcast-only, it does no routing. Whatever receives the packet will hop it until it reaches the destination.

Channels and user information can be shared over a QR code.

Built-in API and MQTT support, it can be used to link to different services.

Location of the nodes can be "fuzzed".

### Take-Away: Matthew Newhall - Web 2.0 to 3.0
- Centralization has harmed Web 2.0, since all of it is on central servers and networks.
- LoRa and Meshtastic is Web 3.0, since it is decentralizing the communications
- By having decentralized networks and movement toward Web 3.0, it may be possible to enable more enjoyable, meaningful connections
- Web 3.0 can be an "electronic neighborhood". Physical proximity, interconnected and peer-to-peer.
