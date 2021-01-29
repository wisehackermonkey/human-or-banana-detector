# human-or-banana-detector
 simple webpage that uses the webcam to detect if it sees a banana or a human

# Demo  gif of project in action
![](./demo_v2.gif)
# Docker development commands
#### Build
```bash
cd /path/to/project
docker build -t wisehackermonkey/human-or-banana-detector:latest .
```
#### Run Development
```bash
# Bash
docker run -it --rm -v ./website/:/usr/share/nginx/html/ wisehackermonkey/human-or-banana-detector:latest

#powershell
docker run -it --rm -v ${PWD}/website/:/usr/share/nginx/html/ wisehackermonkey/human-or-banana-detector:latest
```

#### Deploy (local or cloud)
```bash
# NOTE -d runs in the background -d=daemon
docker run -it --rm -p 80:80 wisehackermonkey/human-or-banana-detector:latest
# for my system it was
See http://www.orancollins.com:4444/ to view it live as of 20210128
docker run -d --restart=always -p 4444:80 wisehackermonkey/human-or-banana-detector:latest

```
#### deploy docker-compose
```bash
cd ~
git clone https://github.com/wisehackermonkey/human-or-banana-detector.git
cd human-or-banana-detector
docker-compose pull
docker-compose up -d
```
#### push
```bash
docker login
docker push wisehackermonkey/human-or-banana-detector:latest
```

# Maintenance
### this project is not under active maintenance (its a one off project)

# License
### MIT oran c  (c) 2021