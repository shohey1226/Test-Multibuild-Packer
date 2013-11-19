# Multi build with Packer (chef provisioner)


- Packer: http://www.packer.io
- Berkshelf: http://berkshelf.com/index.html

## Installation

1. Install VirtualBox
2. Install vagrant
3. Install pcaker
4. Setup up Berkhself and install cookbooks

    gem install berkshelf
    $ cat > Berksfile
    site :opscode
    
    cookbook 'mysql'
    ^c
    $ berks install --path=./cookbooks 

## How to create images 

    $ packer build packer.json

