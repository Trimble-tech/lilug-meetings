# August 2026 LILUG Meeting
*August 11th, 2026 @ [Digital Ballpark](https://maps.app.goo.gl/Uef2PiZBpZLd1n3QA)*
*Pace-notes by [Chris Trimble](https://github.com/Trimble-tech)*

## News & Small Talk
- Dreamhost hosting for LILUG.org is going to be phased out, so we are considering alternatives
    - Mailing list is on Dreamhost
    - Data will be exported to a new platform, we need to determine a new location to replace Mailman
    - Self hosted versus mailing list service or other asynchronous service
        - Groups.io, or other email services
- AMD Vulkan Linux drivers ported to Windows: (Youtube - Brodie Robinson)[https://www.youtube.com/watch?v=bh8uippvOYA]
- Mozilla revokes signing key for Firefox and Thunderbird (Hacker News)[https://thehackernews.com/2026/08/mozilla-revokes-firefox-and-thunderbird.html?m=1]
- No LILUG Picnic coming up

## Main Discussion: Syncthing by Matthew Newhall
(Syncthing Documentation)[https://docs.syncthing.net/index.html]

- Peer to peer file sharing and syncing
- Uses NAT traversal
- a sync daemon is needed for each device, so there is no client or server
- file versioning is present
- send only or receive only folder
- several clients exist, including [Syncthing-GTK](https://github.com/kozec/syncthing-gtk)