## AmazonStorePrice
This module find the price from url given

Compatible with all amazon store

[![Build Status](https://travis-ci.org/Mirio/amazonstore-price.svg?branch=0.1)](https://travis-ci.org/Mirio/amazonstore-price) [![PyPI](https://img.shields.io/pypi/dm/amazonstoreprice.svg)]() [![Github All Releases](https://img.shields.io/github/downloads/mirio/amazonstoreprice/total.svg)]() [![Documentation Status](https://readthedocs.org/projects/amazonstoreprice/badge/?version=latest)](http://amazonstoreprice.readthedocs.org/en/latest/?badge=latest)


## Requirement
Python 3.x

Python Library = [ 'requests', 'beautifulsoup4' ]

## How to install
```
pip install amazonstoreprice
```

## Install from source
```
git clone https://github.com/Mirio/amazonstoreprice.git
cd amazonstoreprice
python setup.py install
```

## Getting Started

Example:
```
from amazonstoreprice import AmazonStorePrice

url = "http://www.amazon.it/Inside-Out-Ronnie-Del-Carmen/dp/B016LMC90O/" \
      "ref=sr_1_1?ie=UTF8&qid=1455389197&sr=8-1&keywords=inside+out"
pricelib = AmazonStorePrice()
print(pricelib.getprice(url, retry_ontemp=True))
```

Output:
```
$ python example_getprice.py
15.99
```