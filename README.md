# Awesome Playbooks [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of community-sourced playbooks. Hands-on, chapter-based instructional content by practitioners, for practitioners.

## What is a Playbook?

A playbook is a structured, hands-on guide built from real-world experience. Not a link list. Not a wiki. Not a blog post.

Playbooks are:

- **Chapter-based** - Numbered sections that build on each other
- **Practical** - Commands you can run, tools you can use, labs you can build
- **Community-sourced** - Written and maintained by people who do the work
- **Open** - Licensed for sharing and adaptation (typically CC BY-SA 4.0)

## Playbooks

### Security

- [Vessel Hacking Playbook](https://vessel.hackingplaybook.com) - Maritime cybersecurity testing: NMEA 0183/2000, CAN bus attacks, spoofing, bus priority, address claiming. ([source](https://github.com/blackandwhitehat/awesome-hacking-playbook/tree/main/vessel-hacking))
- [IoT Hacking Playbook](https://iot.hackingplaybook.com) - Hardware hacking with Linux: UART, SPI, SWD/JTAG, firmware extraction, Ghidra analysis. ([source](https://github.com/blackandwhitehat/awesome-hacking-playbook/tree/main/iot-hacking))

### Networking

_None yet. [Start one.](#start-your-own-playbook)_

### Hardware

_None yet. [Start one.](#start-your-own-playbook)_

### Software

_None yet. [Start one.](#start-your-own-playbook)_

### Other

_None yet. [Start one.](#start-your-own-playbook)_

## Start Your Own Playbook

Anyone can create a playbook. Here's the structure:

```
your-playbook/
├── README.md              # Overview and table of contents
├── MANIFEST.json          # Chapter listing (auto-generated if using CI)
├── CONTRIBUTING.md        # How others can help
├── 01-introduction.md     # First chapter
├── 02-topic.md            # More chapters (numbered)
├── ...
├── images/                # Diagrams, screenshots
├── tools.md               # Relevant tools
├── lab-setup.md           # Practice environment setup
└── resources.md           # Links and references
```

### MANIFEST.json Format

```json
{
  "id": "your-playbook",
  "title": "YOUR PLAYBOOK TITLE",
  "icon": "🔧",
  "description": "One-line description.",
  "chapters": [
    {"file": "README.md", "title": "Overview", "num": "00"},
    {"file": "01-introduction.md", "title": "Introduction", "num": "01"},
    {"file": "02-topic.md", "title": "Your Topic", "num": "02"}
  ]
}
```

### Guidelines

- Write for practitioners, not academics
- Include actual commands, configs, and examples
- Keep chapters focused on one topic each
- Use numbered filenames (`01-`, `02-`, ...) for ordering
- Put images in an `images/` directory with relative paths
- License openly (CC BY-SA 4.0 recommended)

### Auto-generating MANIFEST.json

Add this [GitHub Action](https://github.com/blackandwhitehat/awesome-hacking-playbook/blob/main/.github/workflows/generate-manifests.yml) to your repo and MANIFEST.json will update automatically when chapters change.

## Submit Your Playbook

Have a playbook that follows this format? Submit a PR adding it to the list above.

Include:

- **Title and link** to the hosted version (if any) or the repo
- **One-line description** of what it covers
- **Source link** to the GitHub repo

## License

CC BY-SA 4.0
