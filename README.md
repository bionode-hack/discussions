
# Software required for Hackathon
During the hackathon, you will be able to use a remote machine already setup with
everything you need (easiest but limited), use a local copy of that machine through [Docker](https://www.docker.com/) (recommended), or install
the software on your local operating system (advanced users).

## How to access remote machines

For simple things, like code examples during a talk, you can go to [try.bionode.io](http://try.bionode.io) and access a machine
through your browser. However, the command line, text editor, and filesystem explorer provided by
the website are very limited and there is no functionality to download or upload your files easily.

For some real hacking, we will provide machines you can ```ssh``` into and mount the filesystem with ```sshfs```.
There's a lot of documentation online on how to get and use ssh for every operating system.

```bash
# Access machine through ssh
ssh -i identity_file.pem remoteuser@your_host_address
# Mount folder
sshfs -o IdentityFile=identity_file.pem remoteuser@your_host_address:/host_location_to_mount /mnt/ec2
```

## How to get software with Docker
Go to [docker.com](https://www.docker.com/) and get [Docker for Mac](https://download.docker.com/mac/beta/Docker.dmg) or [Windows](https://download.docker.com/win/beta/InstallDocker.msi).
For Linux, follow the [distro specific instructions](https://docs.docker.com/engine/installation/linux/).

Then simply run in your terminal:

```bash
docker run --rm -it -v project_folder:/app bionode/try-bionode
```

## How to get sofware locally

### OSX

```bash
# Get and install Homebrew (http://brew.sh) with following command
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
# Install Node.js versions manager
brew install n
# Get latest stable Node.js
sudo n stable
```

### Linux (Ubuntu)

```bash
# Install Node.js package manager
sudo apt-get install npm
# Install Node.js versions manager
sudo npm install -g n
# Get latest stable Node.js
n stable
```

### Windows
Go to [nodejs.org](https://nodejs.org) and follow Windows instructions.

# Presentation slides
* [Node.js Streams in detail](https://github.com/bionode-hack/discussions/blob/master/slides/bionode-hackathon.1.0.tutorial.streams.pdf)

# Online courses

## JavaScript
[Workshopper](http://nodeschool.io/#workshoppers) is the name used for the open source lesson modules associated with [NodeSchool](http://nodeschool.io/). All are self guided (you don't need to attend a workshop to do one) and most work offline.

From all these, we recommend the following (by order of importance for Hackathon):

### Core
These workshoppers focus on essential skills for working with Node.js.
* javascripting - Learn the basics of JavaScript. No previous programming experience required.
* learnyounode - Learn the basics of node: asynchronous i/o, http.
* stream-adventure - Learn to compose streaming interfaces with .pipe().
* git-it - Learn Git and GitHub basics.
* How to npm - Learn how to use and create npm modules.

### Electives
Workshoppers on popular libraries or styles of writing Node.js.
* Functional Javascript - Learn fundamental functional programming features of JavaScript in vanilla ES5.
* Async You - Learn to use the async package.


## Bioinformatics
* [Coursera](https://www.coursera.org/courses?languages=en&query=bioinformatics)

# Books
## JavaScript
* [JavaScript for Cats](http://jsforcats.com/) by [Max Ogden](https://twitter.com/denormalize)
* [Human JavaScript](http://read.humanjavascript.com/) by [Henrik Joreteg](https://twitter.com/HenrikJoreteg)

## Bioinformatics
* [Bioinformatics Data Skills](http://shop.oreilly.com/product/0636920030157.do) by [Vince Buffalo](https://twitter.com/vsbuffalo)


# Useful Node.js modules
## For Streams
* [mississippi](https://github.com/maxogden/mississippi) - a collection of useful stream utility modules
* [multistream](https://github.com/feross/multistream) - multistream is equivalent to executing a bunch of commands in sequence in bash
* [multi-read-stream](https://github.com/mafintosh/multi-read-stream) - multi-read-stream is like forking a bunch of processes and reading their output in parallel
* [multi-write-stream](https://github.com/mafintosh/multi-write-stream) - multi-write-stream is forking a bunch of process but writing to them all in parallel

## For accessing data
* [Request](https://github.com/request/request) - Simplified HTTP client

## For Web Scrapping
* [Casper.js](http://casperjs.org/) - Navigation scripting & testing for PhantomJS and SlimerJS

## Bionode
* [bionode-template](https://github.com/bionode/bionode-template) - A base template for quickly creating bionode modules.
* [bionode-ncbi](https://github.com/bionode/bionode-ncbi) - Node.js module for working with the NCBI API (aka e-utils).

# Streams 
## Quickstart
This is an example of how you can quickly write a Stream in Node.js

```javascript
var through = require('through2')
var stream = through2.obj(transform)
function transform (obj, enc, next) {
  // do things, example:
  var self = this
  requestSomethingFromDB(obj.name, function(data) {
    obj.data = data
    self.push(obj)
    next()
  })
 }
```

## Tutorials
* [Using streams - readable, writable, transform streams and flow control](http://blog.yld.io/2016/01/13/using-streams) by [Pedro Teixeira](https://twitter.com/pgte)
* [The Stream Handbook](https://github.com/substack/stream-handbook) by [James Halliday](http://substack.net/)
