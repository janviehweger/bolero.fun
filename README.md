# CarrIOTA Bolero

Bolero is a desktop application for various environments (Windows, Mac, Linux) to easily
run an IOTA full node.

## Table of contents

  * [Getting Started](#getting-started)
    * [Prerequisites](#prerequisites)
    * [Installing](#installing)
    * [Running](#running)
    * [Shutting Down](#shutting-down)
  * [Building Locally](#building-locally)
  * [FAQ](#faq)
  * [Contributing](#contributing)
    * [Donations](#donations)
    * [Running Bolero](#running-bolero)
  * [Authors](#authors)
  * [License](#license)

## Getting Started

These instructions will get you a copy of this project running on your machine.

### Prerequisites

You need Java to have installed on your machine.

You also need to open ports (port forwarding) in your NAT Router:

* **UDP 14600**
* **TCP 15600**
* **TCP 16600**

Please refer to your Router's manual on how to do that.

### Installing

Download a package corresponding to your OS from releases, unpack, click the executable.
On Linux, you might need to start bolero.run from the command line.

### Running

There is not much to do here. This is still barebone. Just start the app.
Everything runs on default ports and cofigurations.

The app appears as a carrot symbol in your tray/task bar.

First start might take a while, since Bolero downloads IRI (full node package)
and a snapshot of the database, which is over 5GB in size. So the first start
might take some time.

Once Bolero is running as is synced, you can use it as a full node for your
IOTA wallet with this address:

```
http://localhost:14265
```

### Shutting Down

Right click on the carrot in your tray/task bar and select "Exit".

## Building locally

```
npm install
npm run build

# Run development version
npm run dev

# Package binaries
npm run package
```

## FAQ

### How to upgrade?

Shut down Bolero, download the new version. Start it. Database and snapshots are preserved.

### Where is the database located?

In the User's home directory in a folder called ```.bolero```

### It takes very long to get synced

The longer you have been offline (not running Bolero), the longer it takes.
Also, make sure that your ports are open (refer to the prerequisites instructions above.)

### What if I have more questions?

* Join ```#bolero``` channel on IOTA's slack!

## Contributing

### Donations

**Donations always welcome**:

```
IQJGHISHRMV9LEAEMSUIXMFTLLZIJWXIQOAZLGNXCFY9BLPTFTBNBPGU9YQFQKC9GEBPNNFO9DMGKYUECCG9ZSHMRW
```

### Running Bolero

THe longer your app is running, the better for the network. Contribute to IOTA
by running Bolero as much as you can!


## Authors

* **Roman Semko** - *SemkoDev* - (https://github.com/romansemko)

## License

This project is licensed under the ICS License - see the [LICENSE.md](LICENSE.md) file for details

