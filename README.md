[![Build Status](https://travis-ci.org/garethahealy/travisci-vagrant.svg?branch=master)](https://travis-ci.org/garethahealy/travisci-vagrant)
[![License](https://img.shields.io/hexpm/l/plug.svg?maxAge=2592000)]()

# travisci-vagrant
PoC to see if its possible to build/test vagrant images on travis-ci.org

## Concept
See .travis.yml for more info on what needs to be installed.

## Works?
Sadly not. vagrant/virtualbox needs VT-x enabled, travis currently doesnt seem to support this, as build fails with:

    VBoxManage: error: VT-x is not available (VERR_VMX_NO_VMX)
