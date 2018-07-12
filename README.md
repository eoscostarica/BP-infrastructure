
<p align="center">
	<a href="https://git.io/col">
		<img src="https://img.shields.io/badge/%E2%9C%93-collaborative_etiquette-brightgreen.svg" alt="Collaborative Etiquette">
	</a>
	<a href="https://discord.gg/bBpQHym">
		<img src="https://img.shields.io/discord/447118387118735380.svg?logo=discord" alt="chat on Discord">
	</a>
	<a href="https://discord.gg/bBpQHym">
		<img src="https://img.shields.io/discord/447118387118735380.svg?logo=discord" alt="chat on Discord">
	</a>
	<a href="https://twitter.com/intent/follow?screen_name=eoscostarica">
		<img src="https://img.shields.io/twitter/follow/eoscostarica.svg?style=social&logo=twitter" alt="follow on Twitter">
	</a>
</p>

# Block Producer Technical Info and Architecture

<div align="center">
  <img src="https://github.com/eoscostarica/block-producer-architecture/blob/master/img/eos-costa-rica.png" />
</div>

This document is intended as a open discussion with the EOS community and
we encourage suggestions. Please let us know how we can better leverage the
resources in Costa Rica to support EOS. We want your feedback!

We are constantly thinking of ways to improve our infrastructure and have outlined the following [Technical Roadmap](https://eoscostarica.com/documents/EOS-costaRica-document-tech.pdf)  , we will actively adapt our roadmap to network conditions and add capacity / redundancy as needed.

<div align="center">
  <img src="https://github.com/eoscostarica/block-producer-architecture/blob/master/img/illustration-network-2-black.jpg" />
</div>

## Bare Metal Servers Specs ##
                           
### Primary and secondary block producer nodes : ###

- <b>4 x CPU 24 cores</b> (48 threads) @ 1.87GHz
- <b>512 GB RAM</b>
- <b>8TB SSD Storage</b> in RAID 5
- <b>100 MBps uplink</b>
                            
We want to do our part to ensure the EOS network scales as smoothly as possible. We will allocate block rewards towards improving our hardware as one of our initial priorities in order to handle a large number of transactions and have redundant equipment ready to go at a moments notice. We envision the following scaling plan for hardware:

- <b>2 x CPU 28 cores</b> (total 56 Cores and 112 threads) @ 2.50 GHz
- <b>1.5TB GB RAM </b> DDR4–2666mhz 
- <b>8TB SSD Storage</b> in RAID 5
- <b>1GBs uplink</b>

### Load Balanced Full Nodes : ###

We have provisioned two servers as load-balanced full nodes with our initial hardware setup to shield our producer nodes and respond in a timely manner to requests coming from users in our region. The number of nodes can be easily increased as demand increases.

In addition to providing reliable API endpoints used to query the EOS blockchain we plan to allow users to host files and query application databases. These services will become vital for applications to get the information they need without having to run and maintain their own scalable hosting services.

We look forward to the EOS token holder's support in order to continue with the deployment of full nodes to serve the demand of Dapps used by millions of users in Central and South America.

## Network Redundancy ##

Fiber optic connections reach Costa Rica on both Pacific and Caribbean coasts via three submarine cables that provide the majority of bandwidth to Costa Rica. Access to all three backbones, <i> ARCOS-1, MAYA-1, and Pan American Crossing (PAC) </i> provides real time fail-over and redundancy at our facility. Additionally all 6 Central American nations are interconnected via a terrestrial fiber optic network <i>(REDCA)</i>. Direct connections to all upstream carriers ensure that no single point of failure is present in the network. 

<div align="center">
  <img style="width: 50%; float:right; " src="https://github.com/eoscostarica/block-producer-architecture/blob/master/img/network-redundancy.png" />
</div>

The network employs BGP to assure all traffic reaches its destination if one connection fails. Communication to international connections is made fully redundant and supported in two locations, our main building in San Jose and the Teleport in Calle Blancos, approximately 7 kms away. 

The EOS network will benefit from this infrastructure, which includes private peering network connections to major Internet carriers. These private peering arrangements allow the network to quickly and efficiently exchange packets of data with every major backbone carrier in a one-to-one environment.

[Official Website - eoscostarica.io](http://eoscostarica.io)  