electron-video-stream
-----------------------

Use electron to stream video to the Internet.

How it works

* Use electron to capture the video stream
* webRTC to create connection

Usage
=====

### Installation

`npm install electron-video-stream -g` to install the command

### How to run

You need to define the peer ID from the command line so that the client knows who to call

```
$ electron-video-stream 'wcl-pi'
```

And then you can find the video at https://fraserxu.me/electron-video-stream?wcl-pi

Development
==============

`npm install` to install all the dependencies

`npm run build` to build the code for client

`npm run watch` to auto build code

`./cli.js wcl-pi` to start electron from the command line

You may also need to run `chmod +x cli.js` to make it executable.

### To publish

I use gh-pages to host static page.

```
git checkout gh-pages
git reset --hard origin/master
git add --all
git commit -m 'gh-pages update'
git push origin gh-pages
```

License
=======
MIT
