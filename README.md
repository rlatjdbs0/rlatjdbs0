#!/bin/bash

pushd /tmp

apt-get install -y curl wget
wget http://media.steampowered.com/client/installer/steam.deb
dpkg -i steam.deb
apt-get install -yf

popd
