---
layout: default
title: VBAN Object
parent: VMR Class
nav_order: 4
---
# `vban` object

Use this object to control VoiceMeeter’s VBAN interface.

---
##### for a list of all `vban` parameters, check out [VBVMR docs](http://download.vb-audio.com/Download_CABLE/VoicemeeterRemoteAPI.pdf#page=17)

## Set any parameter

```lua
    voicemeeter.vban.enable:= true

    voicemeeter.vban.instream[1].ip:= "192.168.0.122"
    voicemeeter.vban.instream[1].port:= "5959"
    voicemeeter.vban.instream[1].on:= true
    
    voicemeeter.vban.outstream[3].name:= "defStream"
    voicemeeter.vban.outstream[3].quality:= 4
    voicemeeter.vban.outstream[3].bit:= 2
```

## Retrieve any parameter
```lua
    stream_channels:= voicemeeter.vban.instream[2].channel
```
