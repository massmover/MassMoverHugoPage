---
title: "Commander Multi-Bot"
date: "2019-01-09"
author: "Auyer"
---

This is an OpenSource Project available on Github:
<a href="https://github.com/auyer/commanderBot"><img src="/img/Octocat.png" height="300" alt="GitHub Logo"></a>

The CommanderBot is a Multi-Token Discord Bot.
This can be used to split intensive operations, or API limited opperations like the "User Voice Channel Move" opperation (limited by the API). 

Is is capable of using N "Servant" Bot connections to perform fast mass "User Move" operations, and the request will be executed by the ammount of bots connected to the server.

## Configuration

Get your Discord Bot tokens (at least one) in the [official developers portal](https://discordapp.com/developers)

The first one should be in the "CommanderToken" slot in the config file.
The rest will be the servant Tokens, and should be added in a List.

The Permission integer must be 16780288 (Move, Read messages, and Write messages).

## Installation
You can get the lastest binary here: (soon)

## Building Yourself
```go
go get -u github.com/auyer/commanderBot
```
Build using 
```go
go build .
```
If you want to cross compile it to run in a different OS or architecturte (like a rapberry pi), do:
```go
CGO_ENABLED=0 CC=arm-linux-gnueabi-cc GOOS=linux GOARCH=arm GOARM=6 go build .
```

<style>.bmc-button img{width: 27px !important;margin-bottom: 1px !important;box-shadow: none !important;border: none !important;vertical-align: middle !important;}.bmc-button{line-height: 36px !important;height:37px !important;text-decoration: none !important;display:inline-flex !important;color:#ffffff !important;background-color:#FF813F !important;border-radius: 3px !important;border: 1px solid transparent !important;padding: 1px 9px !important;font-size: 22px !important;letter-spacing:0.6px !important;box-shadow: 0px 1px 2px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;margin: 0 auto !important;font-family:'Cookie', cursive !important;-webkit-box-sizing: border-box !important;box-sizing: border-box !important;-o-transition: 0.3s all linear !important;-webkit-transition: 0.3s all linear !important;-moz-transition: 0.3s all linear !important;-ms-transition: 0.3s all linear !important;transition: 0.3s all linear !important;}.bmc-button:hover, .bmc-button:active, .bmc-button:focus {-webkit-box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;text-decoration: none !important;box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;opacity: 0.85 !important;color:#ffffff !important;}</style><link href="https://fonts.googleapis.com/css?family=Cookie" rel="stylesheet"><a class="bmc-button" target="_blank" href="https://www.buymeacoffee.com/auyer"><img src="https://www.buymeacoffee.com/assets/img/BMC-btn-logo.svg" alt="Buy me a coffee"><span style="margin-left:5px">Buy me a coffee</span></a>