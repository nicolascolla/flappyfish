# Flappy Fish
![](icon.png)

Ubuntu Touch HTML5 game based on the work of [shuding](https://github.com/shuding/flappybird).

[![OpenStore](https://open-store.io/badges/en_US.png)](https://open-store.io/app/flappyfish.collaproductions)
[![](https://i.imgur.com/KIipzE8.png)](https://t.me/collaproductions)

### Building the app (Ubuntu-based distros)

Install [clickable](https://clickable-ut.dev/en/latest/install.html):

```
$ sudo add-apt-repository ppa:bhdouglass/clickable
$ sudo apt-get install clickable
```

Clone this repository and build:

```
$ git clone https://github.com/nicolascolla/flappyfish.git
$ cd flappyfish/flappyfish
$ clickable build
```

### Building instructions for 16.04

Install [clickable](https://clickable-ut.dev/en/latest/install.html):

```
$ sudo add-apt-repository ppa:bhdouglass/clickable
$ sudo apt-get install clickable
```

Clone this repository, change the framework and build:

```
$ git clone https://github.com/nicolascolla/taptaptap.git
$ cd flappyfish/flappyfish
$ sed -i 's/ubuntu-sdk-20.04/ubuntu-sdk-16.04.5/' clickable.json
$ sed -i 's/20.04/16.04/' flappyfish.apparmor
$ clickable build
```

You can play the game on any web browser by opening flappyfish/www/index.html.

### Known bugs in older Ubuntu versions

-The game starts with a "Game Over" screen instead of the usual "Get Ready!"

-Being an HTML5 app, it will tend to be slow on low-end devices (at least until the Ubuntu Touch webview is improved).

-The fish can get stuck jumping upwards until the game is restarted.

These bugs should be solved in Focal.

### Screenshots

![](screenshot.png)
