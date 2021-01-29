# human-or-banana-detector
 simple webpage that uses the webcam to detect if it sees a banana or a human



# Docker development commands
#### Build
```bash
cd /path/to/project
docker build -t wisehackermonkey/human-or-banana-detector:latest .
```
#### Run
```bash
# Bash
docker run -it --rm -v ./website/:/usr/share/nginx/html/ wisehackermonkey/human-or-banana-detector:latest

#powershell
docker run -it --rm -v ${PWD}/website/:/usr/share/nginx/html/ wisehackermonkey/human-or-banana-detector:latest
```
