# WolfshadeMud

## Preprequisites
### Fedora
```
# dnf install autoconf gcc gcc-c++
```

### Ubuntu/Debian
```
# apt-get install make autoconf gcc g++ 
```

## Build 

```
# cd WolfshadeMud/src/
# autoconf
# ./configure
# make
```

## Starting Server
```
# cd WolfshadeMud/
# touch players/players.wolfshade
# ./bin/wolfshade
```

## Troubleshooting

### Segmentation fault upon new telnet connection
```
wolfshade: ./character.attributes.cpp:112: void CCharacterAttributes::InitStatics(): Assertion `mPlayerFile' failed.
Signal caught: mud shutting down.
```

- Make sure you are starting mud from root source code directory. Starting woflshade from inside bin directory will not work!
