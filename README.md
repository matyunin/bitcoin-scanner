bitcoin-scanner
===============

Multithread python bitcoin wallets scanner for [directory.io](http://directory.io/)


Usage is pretty simple:
```bash
$ python bsc.py
```

Current page number will be saved to ```page``` file for future scanning. All found wallets will be appended as CSV to ```wallets``` file. And if once balance is more than zero - this wallet will be appended to ```wallets_balance``` file.

*Its strongly recommendated to use python 2.**

Required python modules:
```python
import re
import sys
import json
import signal
import requests
import cssutils
import threading

from cssutils import css
from BeautifulSoup import BeautifulSoup
```
