# lily: hosts manager takes effect immediately on switch

![capture](https://cloud.githubusercontent.com/assets/8019222/18225305/4a399b78-7222-11e6-8e1e-9e0037c63d2b.PNG)

## Motivation
We usually have to switch between a bunch of test environments which have same domains but with different IPs.
Since it's troublesome to modify hosts directly, we use some tools to manage it.
I've tried HostAdmin, SwitchHosts! and some others but found that they all have the same problem: browser reboot
is required in order to take effect after switch.

So I decide to solve this problem by "Reinventing the wheel", and as a Go enthusiast, I choose Go to develop it.
If you're interested in this project please fork it and pull request is prefered :)

## Feature
* Takes effect immediately on switch
* Single process
* Realtime notification 
* Written purely in Go
* Clean code

## Roadmap
Only Windows is supported recently and MacOS and Linux will be supported in the near future.
Probably I will use [Electron](http://electron.atom.io/) framework to implement cross-platform feature.

## Build
```
get get -v github.com/tinycedar/lily
go build -ldflags="-H windowsgui"
```
