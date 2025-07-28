# July 2025 LILUG Meeting
*July 8th, 2025 @ [Digital Ballpark](https://maps.app.goo.gl/Uef2PiZBpZLd1n3QA)*
*Pace-notes by [Chris Trimble](https://github.com/Trimble-tech)*

## News & Small Talk
- Critical Sudo Vulnerabilities
    - This was found and patched back in April, but disclosed now
    - There were two separate issues, one with the `--chroot` option and the other with the `-h` (host) option.
    - Generally most systems should no longer be affected as long as they were patched/updated recently.
    - https://thehackernews.com/2025/07/critical-sudo-vulnerabilities-let-local.html

- LILUG Picnic 2: date TBD

## Main Discussion: Lightning Talks
In this meeting, we had several smaller conversations on Linux-related topics.

### Publishing Books on Amazon: Gordon Edward

Have a story or skill to share? Do you want to publish a book about something you are good at? This talk briefly discussed publishing books on Amazon (for example).

**Formatting**
- Full color books need to be 72 pages
- Different Pricing can be present for paperback and electronic (Kindle)
- Margins are automatic in Kindle

**Publishing Info**
- When creating a book, you need to get an ISBN number to publish. If the number is generated from Amazon, it is free but you can only sell the book on Amazon.
- Picking the right topic is important for marketing the book. Linux might be a underneath computers or under programming, for example.
- Search Engine Optimization can be done through keywords as well.
- Amazon asks if AI generated content is anywhere in the book.

**Formatting**
- PDF is the source file needed for paperback, while Kindle has a proprietary format.
- Manuscripts can be created wuth PDF, docx, rtf, etc. and cover the interior contents of the book.
- Covers can be created by Amazon or created on your own and uploaded as a PDF.

### Matt Lindsey: ncdu
N-Curses DU (ncdu) is a program that views folders within a terminal and can be used to navigate through different directories. The program is meant to present the findings more easily than tools like du.
- Faster and simpler than DU.
- Note that ncdu scans all files in the directory it is run in before launching to understand the layout. With large folders this might take an extended period of time.
- Can be installed on Redhat or Debian distros from the `ncdu` distro.

### Matt Newhall: Undoing CHMOD & CHOWN on a folder
- Use permissions from a similar folder to replicate to the folder needing revert
- 

Or, you can extract permissions from a tarball of a backed up file.

### Yutong: Cryptocurrency Issues and How to Avoid Them
- Cryptocurrency can be a way to make spare income off of a running server where electricity costs and hardware power are allocated cheaply.
- However, scammers or malicious actors can pull the base token or devalue less common currencies to extract value of the coin.
- If the capitalization of the cryptocurrency is low, less money is needed to devalue the currency.

**Possible mitigations:**
- Stick to more mainstream currencies
- It might be possible to use bots or algorithms to automate fraud detection.


### Chris: Markdown Formatting

This is a document written in Markdown, and it has a paragraph. 
This is the same paragraph.

This is a different paragraph.

### Lee: Emby, Plex, and Jellyfin
Emby, Plex, and Jellyfin are all software to store and archive video or audio media.
There are options to categorize media into different libraries.

Emby and Plex are paid applications and have optional features. An example of this is running live TV from a TV tuner or streaming to remote users over the Plex or Emby websites.

A good idea is to pull images like comics and store them in their own library. Lee has created a script to pull RSS feeds for this.

**Transcoding**
- Transcoding is the assembly of the video into playable content.
- This can be done on the server or on the client (like a phone or laptop).
- Transcoding on the server takes CPU and/or GPU power and can be a lot as the users climb. For a lot of home uses, it is good to either use a GPU or a Intel CPU with 4-7th gen (at minimum) or generation. These CPUs are good at handling the media codecs within the CPU itself.

**Handling Media**
- Deciding on a common format like .mkv will help avoid playback issues.
- If using different formats, make sure they are supported by your server stack and the clients.
- Tools like Handbrake can be helpful for modifying media itself, while numerous tools are available for editing metadata.

### Yutong: Formatting Mathematics in Markdown

$$
\underset{\text{Einstein Field Equation}
}{R_{\mu\nu} - \frac{1}{2} R g_{\mu\nu} + \Lambda g_{\mu\nu} = \frac{8\pi G}{c^4} T_{\mu\nu}}
$$

### Take-Away

Next month's meeting: Chris Trimble with Package Managers (apt, dnf, yum, flatpak, etc.)