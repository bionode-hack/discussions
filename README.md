
# Programe

**9:30** Arrivals (tea/coffee ...)

**10:00 - 10:10** Introduction to DNAdigest (Fiona or Adrian)

**10:20 - 10:40** Introduction to bionode (Bruno)

**10:40 - 11:00** Genomic data landscape - a focus on accessibility (Adrian)

**11:00 - 11:30** How to build a Node.js package for data fetching (Bruno) - practical session

**11:45 - 13:00** Hack Session I ( 2:15 h session )

**13:00 - 14:00** Lunch break

**14:00 - 16:00** Hack Session II (3 to 4h) aiming for 14:00 to 17:30 session

**16:15 - 16:45** Sessions Feedback

**16:45 - 17:00** Closing remarks (Adrian + Bruno)

# BioHackers
|   |   |   |   |   |
|:-:|:-:|:-:|:-:|:-:|
| [![adamhurst][adamhurst-img]<br>adamhurst][adamhurst-url] | [![Adrian Alexa][adrianalexa-img]<br>Adrian Alexa*][adrianalexa-url] | [![akmoulai][akmoulai-img]<br>Karim Moulai][akmoulai-url] | [![alectronic0][alectronic0-img]<br>Alec Doran-Twyford][alectronic0-url] | [![beatrix7][beatrix7-img]<br>beatrix7][beatrix7-url] |
| [![beechware][beechware-img]<br>beechware][beechware-url] | [![bmpvieira][bmpvieira-img]<br>bmpvieira*][bmpvieira-url] | [![bunnybooboo][bunnybooboo-img]<br>David Ross][bunnybooboo-url] | [![cachemoi][cachemoi-img]<br>Maximilien Rothier Bautzer][cachemoi-url] | [![clarkie][clarkie-img]<br>Clarkie][clarkie-url] |
| [![ClaudiuCreanga][ClaudiuCreanga-img]<br>Claudiu Creanga][ClaudiuCreanga-url] | [![cwhicher][cwhicher-img]<br>Charlotte*][cwhicher-url] | [![DennisSchwartz][DennisSchwartz-img]<br>Dennis Schwartz*][DennisSchwartz-url] | [![ercekal][ercekal-img]<br>Erce Kalabalikoglu][ercekal-url] | [![fsdev][fsdevlondon-img]<br>fsdev][fsdevlondon-url] |
| [![giovannic][giovannic-img]<br>Giovanni][giovannic-url] | [![glyndk][glyndk-img]<br>Fiona Nilsen*][glyndk-url] | [![halimat94][halimat94-img]<br>Halimat Afolabi][halimat94-url] | [![IsmailM][IsmailM-img]<br>Ismail Moghul][IsmailM-url] | [![Istar-Eldritch][Istar-Eldritch-img]<br>Ruben Paz*][Istar-Eldritch-url] |
| [![jamesbrown0][jamesbrown0-img]<br>James Brown][jamesbrown0-url] | [![jessica-jordan][jessica-jordan-img]<br>jessica][jessica-jordan-url] | [![julns][julns-img]<br>julns][julns-url] | [![Knorcedger][Knorcedger-img]<br>Achilleas Tsoumitas][Knorcedger-url] | [![kynan][kynan-img]<br>Florian Rathgeber][kynan-url] |
| [![lailaPanda][lailaPanda-img]<br>lailaPanda][lailaPanda-url] | [![lmmx][lmmx-img]<br>Louis Maddox][lmmx-url] | [![lorenzorietti][lorenzorietti-img]<br>lorenzorietti][lorenzorietti-url] | [![mcarmenjc][mcarmenjc-img]<br>MCarmen Jimenez Campos][mcarmenjc-url] | [![podderka][podderka-img]<br>podderka][podderka-url] |
| [![pontikos][pontikos-img]<br>Nikolas Pontikos][pontikos-url] | [![pulverizers][pulverizers-img]<br>pulverizers][pulverizers-url] | [![raquelsofi][raquelsofi-img]<br>raquelsofi][raquelsofi-url] | [![rjs-repos][rjs-repos-img]<br>rjs-repos*][rjs-repos-url] | [![SebastianPlace][SebastianPlace-img]<br>Sebastian Place*][SebastianPlace-url] |
| [![shun-liang][shun-liang-img]<br>Shun Liang][shun-liang-url] | [![shyamrallapalli][shyamrallapalli-img]<br>Shyam Rallapalli][shyamrallapalli-url] | [![simplesquare1][simplesquare1-img]<br>Jana Grajciarova][simplesquare1-url] | [![sureshhewabi][sureshhewabi-img]<br>sureshhewa][sureshhewabi-url] | [![uhaz1][uhaz1-img]<br>uhaz1][uhaz1-url] |
| [![vince-lynch][vince-lynch-img]<br>Vince Lynch][vince-lynch-url] | [![wendychanhk][wendychanhk-img]<br>Wendy Chan][wendychanhk-url] | [![yumary][yumary-img]<br>yumary][yumary-url]
<small>35 participants + 8 organizers*</small>

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


<!-- Links -->
<!-- adamhurst  -->
<!-- [adamhurst-img]: https://avatars1.githubusercontent.com/u/9249368?v=3&s=70 -->
[adamhurst-img]: https://avatars1.githubusercontent.com/u/20296888?v=3&s=70
[adamhurst-url]: https://github.com/adamhurst
<!-- Adrian Alexa -->
[adrianalexa-img]: https://avatars2.githubusercontent.com/u/1910746?v3&s=70
[adrianalexa-url]: https://github.com/adrianalexa
<!-- Karim Moulai -->
[akmoulai-img]: https://avatars2.githubusercontent.com/u/11056265?v=3&s=70
[akmoulai-url]: https://github.com/akmoulai
<!-- Alec Doran-Twyford -->
[alectronic0-img]: https://avatars3.githubusercontent.com/u/3073565?v=3&s=70
[alectronic0-url]: https://github.com/alectronic0
<!-- beatrix7 -->
<!-- [beatrix7-img]: https://avatars1.githubusercontent.com/u/11467427?v=3&s=70 -->
[beatrix7-img]: https://avatars1.githubusercontent.com/u/20296888?v=3&s=70
[beatrix7-url]: https://github.com/beatrix7
<!-- beechware -->
[beechware-img]: https://avatars1.githubusercontent.com/u/6025734?v=3&s=70
[beechware-url]: https://github.com/beechware
<!-- Bruno Vieira -->
[bmpvieira-img]: https://avatars1.githubusercontent.com/u/263386?v=3&s=70
[bmpvieira-url]: https://github.com/bmpvieira
<!-- David Ross -->
[bunnybooboo-img]: https://avatars2.githubusercontent.com/u/5793295?v=3&s=70
[bunnybooboo-url]: https://github.com/bunnybooboo
<!-- Maximilien Rothier Bautzer -->
[cachemoi-img]: https://avatars0.githubusercontent.com/u/13235361?v=3&s=70
[cachemoi-url]: https://github.com/cachemoi
<!-- Clarkie -->
[clarkie-img]: https://avatars1.githubusercontent.com/u/2292639?v=3&s=70
[clarkie-url]: https://github.com/clarkie
<!-- Claudiu Creanga -->
[ClaudiuCreanga-img]: https://avatars3.githubusercontent.com/u/7690659?v=3&s=70
[ClaudiuCreanga-url]: https://github.com/ClaudiuCreanga
<!-- Charlotte -->
<!-- [cwhicher-img]: https://avatars1.githubusercontent.com/u/15735131?v=3&s=70 -->
[cwhicher-img]: https://avatars1.githubusercontent.com/u/20296888?v=3&s=70
[cwhicher-url]: https://github.com/cwhicher
<!-- Dennis Schwartz -->
[DennisSchwartz-img]: https://avatars2.githubusercontent.com/u/2827690?v=3&s=70
[DennisSchwartz-url]: https://github.com/DennisSchwartz
<!-- Erce Kalabalikoglu -->
[ercekal-img]: https://avatars0.githubusercontent.com/u/19410057?v=3&s=70
[ercekal-url]: https://github.com/ercekal
<!-- fsdevlondon -->
[fsdevlondon-img]: https://avatars1.githubusercontent.com/u/20030083?v=3&s=70
[fsdevlondon-url]: https://github.com/fsdevlondon
<!-- Giovanni -->
[giovannic-img]: https://avatars2.githubusercontent.com/u/2605711?v=3&s=70
[giovannic-url]: https://github.com/giovannic
<!-- Fiona Nilsen -->
[glyndk-img]: https://avatars1.githubusercontent.com/u/3482363?v=3&s=70
[glyndk-url]: https://github.com/glyndk
<!-- Halimat Afolabi -->
<!-- [halimat94-img]: https://avatars0.githubusercontent.com/u/14026709?v=3&s=70 -->
[halimat94-img]: https://avatars1.githubusercontent.com/u/20296888?v=3&s=70
[halimat94-url]: https://github.com/halimat94
<!-- Ruben Paz -->
[Istar-Eldritch-img]: https://avatars0.githubusercontent.com/u/3746468?v=3&s=70
[Istar-Eldritch-url]: https://github.com/Istar-Eldritch
<!-- Ismail Moghul -->
[IsmailM-img]: https://avatars2.githubusercontent.com/u/5578375?v=3&s=70
[IsmailM-url]: https://github.com/IsmailM
<!-- James Brown -->
<!-- [jamesbrown0-img]: https://avatars2.githubusercontent.com/u/10291002?v=3&s=70 -->
[jamesbrown0-img]: https://avatars1.githubusercontent.com/u/20296888?v=3&s=70
[jamesbrown0-url]: https://github.com/jamesbrown0
<!-- jessica -->
[jessica-jordan-img]: https://avatars2.githubusercontent.com/u/8811742?v=3&s=70
[jessica-jordan-url]: https://github.com/jessica-jordan
<!-- julns -->
[julns-img]: https://avatars0.githubusercontent.com/u/4550264?v=3&s=70
[julns-url]: https://github.com/julns
<!-- Achilleas Tsoumitas -->
[Knorcedger-img]: https://avatars2.githubusercontent.com/u/16969?v=3&s=70
[Knorcedger-url]: https://github.com/Knorcedger
<!-- Florian Rathgeber -->
[kynan-img]: https://avatars3.githubusercontent.com/u/346079?v=3&s=70
[kynan-url]: https://github.com/kynan
<!-- lailaPanda -->
<!-- [lailaPanda-img]: https://avatars0.githubusercontent.com/u/20362728?v=3&s=70 -->
[lailaPanda-img]: https://avatars1.githubusercontent.com/u/20296888?v=3&s=70
[lailaPanda-url]: https://github.com/lailaPanda
<!-- Louis Maddox -->
[lmmx-img]: https://avatars3.githubusercontent.com/u/2979452?v=3&s=70
[lmmx-url]: https://github.com/lmmx
<!-- lorenzorietti -->
<!-- [lorenzorietti-img]: https://avatars3.githubusercontent.com/u/20362617?v=3&s=70 -->
[lorenzorietti-img]: https://avatars1.githubusercontent.com/u/20296888?v=3&s=70
[lorenzorietti-url]: https://github.com/lorenzorietti
<!-- MCarmen Jimenez Campos -->
[mcarmenjc-img]: https://avatars0.githubusercontent.com/u/7700395?v=3&s=70
[mcarmenjc-url]: https://github.com/mcarmenjc
<!-- podderka -->
<!-- [podderka-img]: https://avatars1.githubusercontent.com/u/14463543?v=3&s=70 -->
[podderka-img]: https://avatars1.githubusercontent.com/u/20296888?v=3&s=70
[podderka-url]: https://github.com/podderka
<!-- Nikolas Pontikos -->
[pontikos-img]: https://avatars1.githubusercontent.com/u/3852020?v=3&s=70
[pontikos-url]: https://github.com/pontikos
<!-- pulverizers -->
[pulverizers-img]: https://avatars2.githubusercontent.com/u/8087472?v=3&s=70
[pulverizers-url]: https://github.com/pulverizers
<!-- raquelsofi -->
<!-- [raquelsofi-img]: https://avatars2.githubusercontent.com/u/20362153?v=3&s=70 -->
[raquelsofi-img]: https://avatars1.githubusercontent.com/u/20296888?v=3&s=70
[raquelsofi-url]: https://github.com/raquelsofi
<!-- Richard Shaw -->
[rjs-repos-img]: https://avatars1.githubusercontent.com/u/19165756?v=3&s=70
[rjs-repos-url]: https://github.com/rjs-repos
<!-- Sebastian Place -->
[SebastianPlace-img]: https://avatars3.githubusercontent.com/u/6838875?v=3&s=70
[SebastianPlace-url]: https://github.com/SebastianPlace
<!-- Shun Liang -->
[shun-liang-img]: https://avatars2.githubusercontent.com/u/1120723?v=3&s=70
[shun-liang-url]: https://github.com/shun-liang
<!-- Shyam Rallapalli -->
[shyamrallapalli-img]: https://avatars1.githubusercontent.com/u/3543099?v=3&s=70
[shyamrallapalli-url]: https://github.com/shyamrallapalli
<!-- Jana Grajciarova -->
[simplesquare1-img]: https://avatars0.githubusercontent.com/u/13767979?v=3&s=70
[simplesquare1-url]: https://github.com/simplesquare1
<!-- sureshhewa -->
[sureshhewabi-img]: https://avatars3.githubusercontent.com/u/5387193?v=3&s=70
[sureshhewabi-url]: https://github.com/sureshhewa
<!-- uhaz1 -->
<!-- [uhaz1-img]: https://avatars2.githubusercontent.com/u/4403796?v=3&s=70 -->
[uhaz1-img]: https://avatars1.githubusercontent.com/u/20296888?v=3&s=70
[uhaz1-url]: https://github.com/uhaz1
<!-- Vince Lynch -->
[vince-lynch-img]: https://avatars2.githubusercontent.com/u/16373282?v=3&s=70
[vince-lynch-url]: https://github.com/vince-lynch
<!-- Wendy Chan -->
[wendychanhk-img]: https://avatars2.githubusercontent.com/u/12168646?v=3&s=70
[wendychanhk-url]: https://github.com/wendychanhk
<!-- yumary -->
<!-- [yumary-img]: https://avatars3.githubusercontent.com/u/20368671?v=3&s=70 -->
[yumary-img]: https://avatars1.githubusercontent.com/u/20296888?v=3&s=70
[yumary-url]: https://github.com/yumary
