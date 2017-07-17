In short, if you want the optimal online gaming experience, go to Advanced tab of your Ethernet adapter settings, and disable the following:
* Interrupt Moderation - clumps packets together and sends them as a batch - the main offender
* Flow Control - sounds counterintuitive to disable it, but it messes with existing flow control in Windows networking stack
* Receive Side Scaling - also messes with Windows networking stack
* [anything goes here] Checksum Offload - supposed to speed up performance by offloading TCP/UDP checksumming to hardware; in reality does nothing for an average desktop PC except interfere with Windows networking stack
* Green Ethernet - performance-eating eco garbage
* Priority & VLAN=Disabled (optional needs more tests)


Research:
https://www.speedguide.net/articles/network-adapter-optimization-3449
https://www.speedguide.net/articles/gaming-tweaks-5812