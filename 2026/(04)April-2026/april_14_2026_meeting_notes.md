# April 2026 LILUG Meeting
*April 14th, 2026 @ [Digital Ballpark](https://maps.app.goo.gl/Uef2PiZBpZLd1n3QA)*

*Pace-notes by [Chris Trimble](https://github.com/Trimble-tech)*

## News & Small Talk
- Discussion on Proxmox and Virtualization
- Possible cure for colon cancer
- [LILUG Hangout: Top Golf at 8pm on Tuesday April 21st](https://lilug.org/)
- AI submissions of code and bugs in open-source
- [French government announces planned switch to Linux, likely Gendbuntu, for all government workstations](https://www.zdnet.com/article/france-leaves-windows-for-linux-desktop/)
- Privacy and age-verification
- Web 1.0 vs Web 3.0
    - Meshtastic and related peer-to-peer protocols

## Main Discussion: "Complexity and the Practical Human Solution" by Gordon F. Edward
With evolving tech, management of data and files is getting ever more complex.
Everyone presents thier own conventions but ultimately it is easy to make things complex.
This talk aims to present a possible answer with takeaways that can be adapted towards your approach, regardless of what data you have or where it is stored.

1. Complexity is not just annoying; it is a metaphyiscal law.
2. Everything that works starts simple.
3. Systems grow more tangled no matter how careful you are.
4. This is the fundamental challenge of all organized structures.

### Spegetti Graph Effect
- Clean start: a new Obsidian vault or project
- Structure breaks: add plugins, add notes, and complexity explodes
- Organization trap: more time organizing than working
- Ubiquitous: files, passwords, and more are involved

### Rock Solid Organizational Theories
**Gall's Law**: Complex systems that work invariably evolved from simple systems that work.

**Tesler's Law**: You can't delete complexity-you can only move it around.

**Ashby's Law**: Your  organizing system must be at least as complex as the mess it is trying to manage.

**Functional Information**: Systems naturally grow more complex when they are under selection for usefulness.

### The Key Insight: Hard Limits

#### Digital Space (AI/Computer)
- Limit: 
    - Context Window
    - Computing Power
    - File system limits on characters, size of file, naming
- Constraint: 
    - Token capacity per request
    - Networking
    - Archival/time limits
- Failure: 
    - Hallucination 
    - Data loss

#### Meat Space (Human)
- Limit: 
    - Time & Energy
    - Knowledge or learning curve
- Constraint: 
    - Finite cognitive energy
- Failure: 
    - Burnout/overwhelm.

### The Practical Human Solution
- Simple file system conventions over complex apps.
- No complex tagging or deep nesting.
    - While this allows for more context for files it encourages data sprawl. 
- High-level containers that respect cognitive load.
- The goal is clarity, not perfection.

### Top-Level Containers for Clarity
1. At the root level, use only Big, all-caps folders.
2. These are your primary top-level containers.
3. Never nest deeper than one or two layers.
4. Structure provides immediate clarity and reduces friction.

#### Example File Structure
    /root/
    |-    /root/PROJECTS/
    |-    /root/AREAS/
    |-    /root/FINANCES/
    |-    /root/HEALTH/
    |_    /root/ARCHIVE/

When looking at the *Linux file system*, the structure is shallow and intuitive. 
The folders are not deep, and the top-level folders are indicative of the files held below.

### Managing Depth with Johnny Decimal
1. One or two layers deep-nothing more.
2. For deeper projects, use the Johnny Decimal system.
3. Number your folders so they always sort the same way.
4. Predicatable structure means you never lose track.

#### A Johnny Decimal File System
    10-19   FINANCE    
    |-    11  TAX
    |_    12  BANKING
    
    20-29   PROJECTS
    |-    21  LILUG_TALK
    |_    22  APP_DEV


### Respect Your Brain's Limits
1. No plugins. No fancy tags. No extra systems.
    - When moving to different operating systems, tags can get destroyed.
    - Different users may not use the sub-system of organization correctly; simple is better.
2. Just clean, consistent folders that respect your brain.
3. Systems that respect the human brain's processing capacity.
4. This is how you do your own cleanup without adding complexity.

### AI Assistance Within Boundaries
1. AI can help, but only inside these same boundaries.
2. It can estimate task time and token costs.
3. It can suggest the "smartest next thing" when you are stuck.
4. Only works if you keep requests small and respect context windows.

### Call to Action: A Simple Framework
- We need a simple framwork that brings this all together.
- Structure needs to be helpful and not overbearing
- Tools like file system search need good conventions as much as the humans using them
- Complexity is a feature of reality, not a bug.
- Respect the laws of systems (Gall, Tesler, Ashby)
- Build systems that acknowledge human and computational limits

## Take-Away
Systems like the [Johnny Decimal System](https://johnnydecimal.com/) can be used to prevent nesting or simplify the categorization of files.

- If a file is difficult or impossible to access in Linux, *Midnight Commander* is a program that can access it more commonly.
    - This program interfaces at a kernel level, not a shell level

- In Windows, PowerShell will help deleting files with the `del` command and pressing tab to complete the filename.

- Another take on file structure is demonstrated by Amazon S3 storage; file names have strings and there are no folders.