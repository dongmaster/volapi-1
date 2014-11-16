Volafile-API version 0.1
============

Requires the websocket-client and requests packages.
```
pip3 install websocket-client
pip3 install requests
```

Example:

```python
from volapi import Room
beepi = Room("BEEPi", "ptc")
beepi.postChat("kek")
beepi.uploadFile("shekel.jewpeg")
for msg in beepi.getChatLog():
    print(msg.nick + ": " + msg.msg)
beepi.close()
```
