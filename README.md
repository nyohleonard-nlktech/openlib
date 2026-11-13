# OpenLib

An offline educational library concept for sharing learning resources over a local network.

The website presents a resource hub for students at the University of Bamenda / NAHPI. Its content describes access to lecture notes, past examination papers, and educational videos through a local server, supporting learning where internet access is limited.

## Content
- Educational notes and downloadable resources.
- Past-paper access.
- Embedded educational videos.
- Local-network access concept for campus use.

## Technology
Static HTML and local media folders. A separate local server or campus network configuration is needed to provide resources to multiple devices.

## Run locally
```bash
git clone https://github.com/nyohleonard-nlktech/openlib.git
cd openlib
python -m http.server 8000
```

Visit http://localhost:8000.

## Structure
```text
images/
notes/
videos/
index.html
README.md
```

The page references example paths such as /notes/python.pdf and /videos/intro.mp4. Ensure the referenced files exist before demonstrating downloads or video playback.

## Campus LAN deployment
Run a web server on a host reachable by student devices, configure firewall rules for the chosen port, and provide a stable local IP or DNS name. Test concurrent access and file permissions.

Distribute only resources you are authorized to share. A static page alone does not provide accounts, content management, or access control. No license file is present; all rights reserved unless an explicit license is added.
