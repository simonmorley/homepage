## Intro

A hands-on CTO and software engineer. I love creating solutions for problems that seem impossible to solve. Boring is my mantra - as engineers we all want to learn new stuff but the work-place is the wrong-place for this kind of learning. Learn stuff out of hours, let it inspire your work. Keep work boring.

## Work Stuff

As of November 2022, I'm the CTO at a Crypto exchange called Vaultoro. Since I joined, I've done a bunch of cool software type things that have helped them continue to succeed. Turns out I'm also quite a motivating and driven manager of people.

I've written bots to automate trades and balance their liquidity pools. I re-wrote their entire trading platform and API. Introduced a bunch of new crypto currencies. Added support for FIAT currencies. Wrote some solidity contracts to process inbound and outbound ETH and ERC20 transactions. Hired a bunch of developers. Built and implemented compliance rules and systems so they could get a licence to trade. Integrated a custodian and cold wallet provider to secure their funds. I also helped them release their own stablecoin via an "IBCO".

## Startup Life

Since 2004, I've founded about 5 different startups:

- Cucumber Tony: Cloud-based remote management of WiFi access points
- PolkaSpots: Public WiFi Hotspots and networking installation service
- Perched: AirBnb for kitchens
- Phil: Contactless payment services for homeless people
- [MIMO](https://github.com/mimolabs): Open-source WiFi splash pages and marketing tools

We were in Techstars Berlin 2017 - some of the best times of my startup life were spent between Berlin and Shoreditch. If you were in Techstars too, you can find me on Discord.

The company I currently work at (Vaultoro) was also on the Techstars program and is still 100% in start-up mode :)

## Software languages

I've used the following extensively in production environments:

Golang, Python, Solidity, Javascript, NodeJS, Ruby.

I've also extensively used Postgres, MySQL, Mongo, BigQuery, BigTable, Influx, Redis, Docker, Elasticsearch etc.

### Other stuff:

I love using Jupyter notebooks, Pandas etc. Have done some ML stuff at Cucumber Tony where we were learning from the WiFi data that we'd stored.

I'm currently learning c++. I've written software for embedded devices using c. I'm comfortable with Rust too.

## Devops Stuff

I've automated pretty much everything at all the companies I've worked at using Kubernetes mostly. 

Kubernetes, Google Cloud, CI (Jenkins, Circle, Cloud Builds, GH Actions), Cloudflare.

For the production Kubernetes clusters I've run over the last 5 or so years, I've focused on self-healing services. By ensuring everything will recreate itself after deletion etc, I've managed to keep things running with little or no downtime. I started this approach after using the preemptable instances Google offer - machines that don't live for longer than 24 hours.

Not only does this keep costs down, it *forces* you to build services that recover quickly.

The most complicated deployment was to ensure the certificates for thousands of WiFi devices rotated. If they didn't, it was possible that they'd all go offline. I solved this using kubernetes, pubsub listeners, a bunch of python and letsencrypt.

## Crypto Development

I've spend a couple of years developing Solidity contracts on the Ethereum blockchain. These ranged from proxy contracts, ERC20 contracts and entire platforms to launch a stablecoin, including a couple of NFTs... The deployment of these contracts was mostly done using Hardhat, with some Remix in there too. I've also implemented a Geth node on Kubernetes, and built a bunch of integrations around this. 

For the stablecoin launch, we build a platform which allowed users to swap their 'Cryptos' for sEURO. We also built a bonding service on top of Uniswap's V3 liquidity pool. And we also built a staking service that used ERC721 tokens (aka NFTs) to redeem the 'stakes'.

You can find the repo [here](https://github.com/the-standard/ibco).

Other than Ethereum, I've built numerous systems on other blockchains, include Bitcoin, Litecoin etc.

## Networking

Whilst building Cucumber Tony and PolkaSpots, I had to learn a bunch of networking / UNIX / linux stuff. In fact, since I founded those companies before such things as AWS, I had to do all the server management too. I also wrote some custom pacakges for OpenWRT in c which facilitated the remote management of thousands of WiFi access points around the world. The biggest one was called [Socketman](https://github.com/mylittletony/SocketMan).

One such project, called Rascal, listened for WiFi probes and we were considering using it for some kind of analytics service. However, upon writing this, I realised how intrusive the whole thing was. It was at this point, I decided not to turn Cucumber Tony into an analytics service for moral reasons. There's a link to that [here](https://github.com/mylittletony/rascal).

Our platform mostly used [MQTT](https://mqtt.org/) to communicate with our WiFi devices. I built a Golang based backend to send and receive messages from these devices. It was pretty fun (and stressful) building this. At one point, we had about 5,000 WiFi access points connected to the system.

We also figured out a way for Meraki customers to flash their defunct access points with our firmware. This allowed them to skip all the license costs etc - we weren't so popular with Cisco at the time. Ooops.

## Non Work Stuff

I took a year off to become a professional Ironman. Sadly that didn't work out because COVID caused all the races to be cancelled. But I can however still call myself an Ironman!

I cycle and run pretty much every day. I read a lot of books, anything I can get my hands on really although I did NOT enjoy Ulysses, nor could I finish it.

My family and I have an allotment where we grow a bunch of tasty fruit and vegetables. We also have some bees! I built a "bee monitor" using a raspberry PI.

## This Blog

Originally I built it using markdown, and Gatsby and hosted on Cloudflare's Workers. I guess I really wanted to play with workers and the themes for Gatsby were fab!

As usual, months went by without a blog post. I got an M2 Macbook. When inspiration finally hit, Gatsby wouldn't work. Dependancy hell. I went down the rabbit hole and then remember I'm supposed to be having fun, not fixing stupid issues. 

This is my beef with so much open-source stuff we tend to rely on. It changes so much and, while they mostly all promise to be 'backwards compatible', they rarely are.

So, I'm back on good old Github pages. I like this boring approach to technology.

## My Other Blog

Thinking of putting all my recent posts on Medium, will post a link here when I do.
