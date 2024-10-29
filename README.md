# Dockerize-2048-Game

![mac](https://github.com/user-attachments/assets/80b12450-63b5-452f-a18b-eefcf83ac99e)

## OVERVIEW
A simple project showcasing a web application that serves the classic 2048 game using Nginx within a Docker container.<br>
The Dockerfile efficiently downloads the game files, installs necessary dependencies, and sets up the Nginx server to host the game.

## HOW TO USE
First build the image, make sure you are in the same directory as the Dockerfile.

```bash
docker build -f Dockerfile-Nginx -t game-2048 .
```

Then run the image

```bash
docker run -d -p 80:80 game-2048
```

Finally, access using the url : ( you don't need to specify the port because nginx uses port 80 by default)

```bash
http://localhost
```

Enjoy the game !!


## OPTIONAL ⬇️
I also included an image based on the ubuntu distribution, you are free to use it but you must consider that this image is heavier and takes more storage, I added it just to showcase the fact that we can use different images to build the same app.
