
# Sentivate Network White Paper

![Logo](https://sentivate.com/wp-content/uploads/brizy/3443/assets/images/iW=269&iH=274&oX=0&oY=0&cW=269&cH=274/SNTVTbig.png)

##### TITLE:  SENTIVATE - The Universal Web. 
#####  ABSTRACT
Sentivate is a hybrid web (centralized focused but enhanced by decentralized components) built to be a viable & realistic replacement for the modern web. The network is designed to go beyond the capabilities that any solely centralized or decentralized network could offer. Sentivate addresses the following issues directly: bandwidth crisis, outdated protocols, broken DNS, lack of accountability, lack of identity, reactive security, Domain rules, and web categorization.

##### FOCUS
This white paper is focused on the core network design that serves as the base network & components for Viat, hApps, and the Universal Web. An additional white paper will be released solely on Viat. All technology is focused on ensuring that Sentivate is a revolutionary, and not an evolutionary replacement in modern Internet architecture. 

## INTRODUCTION
##### THE STATE OF THE WORLD WIDE WEB

At present, we find ourselves continuing to utilize a ruinous medium of interconnected communication on a global scale. Humanity’s demands are exponentially increasing of which the World Wide Web simply can’t meet. As we continue to grow, evolve, and venture beyond the solar system, our imperative task becomes revolutionizing the technology we depend on.

The current state of the World Wide Web is deprecationary. If humanity continues to monkey-patch existing problems the Internet will remain the “wild wild west”. Humanity’s ever-increasing demands will never be met by the current state of the Web. We must start thinking in revolutionary terms and not evolutionary. The solution is a complete replacement of contemporary systems, browsers, languages, protocols, and platforms with increased security, speed, efficiency, accountability, trust, identity, capability, and reliability. In order to transition into a new age of information we must replace that which we have become all too comfortable with.

###### BANDWIDTH CRISIS
[Bandwidth is limited, our needs are out growing our networks.](https://www.scientificamerican.com/article/the-bandwidth-bottleneck-that-is-throttling-the-internet/)  To solve this issue we need modern revolutionary technology to replace existing components. If we don’t, fast lanes & prioritization of data is our only option. All those fears that folks have of the repeal of Net Neutrality will be our only hope at keeping the web spinning. The inevitable rise of IoT, more devices per-person, more devices per-household, self-driving cars, car insurance analytics, & developing countries coming online suck up bandwidth we don’t have.

###### THE OUTDATED WEB WE RELY ON IS EATING ITSELF
HTTP & DNS were built a long time ago without the consideration of modern demands in mind. More and more bandwidth is being sucked up, HTTP continues to show its long scalability issues, and DNS is not trustworthy or scalable. If half of the web can be shut down from DoS-ing specific DNS servers there's an obvious architectural problem. HTTP is the current vehicle for money. The entire digital economy is transported over HTTP. Any slowing down to HTTP or DNS means a drastically slower global economy. DNS & HTTP are inherently broken, have poor scalability, are dreadfully slow, lack modern features, eat up bandwidth, and cost consumers & businesses billions. If we don't solve this issue we will experience a massive blow to the economy. When you factor in all the dollar signs one soon realizes that a slower web is a global humanitarian crisis. 

1.  [A one second delay could cost Amazon 1.6BB in sales.](https://www.fastcompany.com/1825005/how-one-second-could-cost-amazon-16-billion-sales)
2.  [_“10 years ago, Amazon found that every 100ms of latency cost them 1% in sales”_](https://www.gigaspaces.com/blog/amazon-found-every-100ms-of-latency-cost-them-1-in-sales/)
3.  [_“Fast forward 10 years later, a 2017 Akamai study shows that every 100-millisecond delay in website load time can hurt conversion rates by 7% – that is a significant drop in sales – 6% – from the time when Amazon first talked about latency in seconds and milliseconds. This goes to show that things aren’t getting any easier for online retailers as user experience is becoming critical to e-commerce success.”_](https://www.akamai.com/us/en/about/news/press/2017-press/akamai-releases-spring-2017-state-of-online-retail-performance-report.jsp)

###### THE FAILURE THAT IS THE DECENTRALIZED WEB AKA WEB 3.0
We know that the global economy requires a performant & inexpensive web. If a solely decentralized web replaced the modern web, then it would accelerate the bandwidth crisis and bring us to a dystopian web. The term Web 3.0 is not a magic globe, a revolutionary idea, or a solution; it's a cash grab. Trades are happening in nanoseconds the global economy doesn't have time to wait seconds or minutes for a block time to verify and then propagate through the network. A replacement for the web shouldn't be slower and more expensive for consumers. Web 3.0 costs more and they like to hide behind things like it's all on-chain and costs very little to launch an app. The reality is, you get what you pay for. Web 3.0 offsets costs to users instead of the services, which also results in a poorer service. Another common argument is to allow users to control their data. That's no problem, say hello to homomorphic encryption. Instead of tackling this issue from just topology, we need to innovate in every aspect of the web and ask more from our web services. The web's topology problem is minor compared to it's outdated technology problem. If these Web 3.0 projects actually cared about changing the web they would focus on the actual issues. **Both topologies have their use cases but together they are a solution to an ever growing problem that has gone unchecked.**

## UNIVERSAL WEB CRYPTOGRAPHY ([SODIUM-NATIVE](https://github.com/sodium-friends/sodium-native))

-  Key Signatures
    -   Single-part signature: Ed25519
    -   Multi-part signature: Ed25519ph
-  Packet Encryption
	- Authenticated Encryption with Additional Data
    - Encrypts a message with a key and a nonce to keep it confidential
    - Computes an authentication tag. This tag is used to make sure that the message, as well as optional, non-confidential (non-encrypted) data, haven’t been tampered with.
    - Encryption: XChaCha20 stream cipher
    - Authentication: Poly1305 MAC

- Key exchange – Shared Session Secret Keys
    - BLAKE2B-512
        - BLAKE2 is a cryptographic hash function **faster than MD5, SHA-1, SHA-2, and SHA-3**, yet is at least as secure as the latest standard SHA-3
        - Optimized for 64-bit platforms—including NEON-enabled ARMs—and produces digests of any size between 1 and 64 bytes
    - X25519 – Ephemeral Key Pair
        - Computes a secret shared between the sender and receiver, using the sender’s secret key and the receiver’s public key (or vice versa)

## HYBRID NETWORK
![Sentivate Hybrid Network](https://sentivate.com/wp-content/uploads/2018/09/hyrbidNetworkTopology.png)

## PROTOCOL

### Universal Data Stream Protocol
###### Data Transport Protocol 

UDSP is a UDP based low-latency, real-time, bi-directional, encrypted, and reliable Data Transport Protocol. 

##### The Problem
As mentioned in the introduction: User’s demands have changed and our requirements of the web have grown. These changes make HTTP a major bottleneck. The HTTP standard itself and TCP are both huge issues. Large data centers moving copious amounts of data from one end-point to the other have latency and cost issues associated with outdated Internet architecture. HTTP is especially problematic when users are experiencing low throughput, limited bandwidth, degraded network connectivity, or requiring a near real-time response. 

##### The Solution
The first step in the construction of the Universal Web is to replace HTTP entirely with UDSP. UDSP is a UDP based low-latency, real-time, bi-directional, encrypted, and reliable Data Transport Protocol. On the Universal Web all communication, streaming, or transferring of any type of data utilizes UDSP. When visiting a site on the Universal Web UDSP is the protocol used instead of HTTP. Specific UDSP client and server modules are required to visit or host a website on the Sentivate Network. UDSP is the foundation and life blood of the Sentivate Network.

UDSP is capable of dynamic reliability on a connection level, or on a per-request basis which is agreed upon between the involved parties. UDSP enforces encryption which means all UDSP connections are encrypted by default, no exceptions. UDSP supports IPv6, Multiplexing, and Multihoming. UDSP relies on cryptographic keypairs and XChaCha20 to establish a connection.

UDSP prioritizes the real-time web and Dispersed Computing. Since connections are bi-directional streams and less chatty this makes the network less clogged and ensures low-latency for the livelihood of the connection. UDSP is far less chatty than HTTP and can be programmatically set to adjust it's own reliability standards. This makes UDSP a highly useful protocol where high-throughput, low-latency, and high reliability are required. Due to UDSP's programmatically dynamic nature, it's efficacious in situations of highly variable and or degraded network connectivity.

UDSP has optional puzzles included in the packets which allow providers and solvers to earn VIAT. Puzzles can vary and thus the puzzles are a Dynamic-Proof-of-Work. The puzzles may be encapsulated or point to data that is required for solving the puzzle. This functionality will be described in the next white paper for VIAT. The puzzles also function as congestion control and a way to limit the potential damages from DDOS attacks. Sentivate turns a typical DDOS attack into profit by the introduction of various puzzle types into packets. When a client solves the served puzzle the client and domain are credited by the network with Viat. If a server is under DDOS attack then the server can dynamically change the reward split up-to 100% for the domain. This ensures the attackers suffer more financial loss and have little to gain. Puzzles ensure that both parties have an incentive to act in good faith. 

![CLIENT CONNECTION](https://sentivate.com/wp-content/uploads/2018/09/DISHyrbid.png)

## UNIVERSAL DOMAIN SYSTEM

### DOMAIN CERTIFICATES
###### ROUTING & CRYPTOGRAPHIC PARAMETERS

Domain certificates provide routing, cryptography, and additional details associated with a hostname. Domain certificates are signed by 3 or more keypairs: Ephemeral, Master, and an authorized Domain Registrar. In order to establish a successful handshake, the domain certificate and a valid signature is required.

The domain's ephemeral certificate also acts as a wallet which stores funds for any puzzles it distributes to clients. A portion of the mined Viat is sent to the ephemeral certificates wallet address. 

### DOMAIN REGISTRAR
###### UPLOAD & SIGN DOMAIN CERTIFICATES

The Domain Registrar, (DR), is used to register a domain and manage a domain's public certificate. The DR validates & signs the public certificates associated with the hostname. The DR then passes the certificate to the Domain Information System which stores the certificate for distribution.


### DOMAIN INFORMATION SYSTEM
###### QUERY DOMAIN ROUTING AND CRYPTOGRAPHY

The Domain Information System, (DIS), returns domain-specific information in the form of a domain certificate from human-readable hostnames. The DIS returns the domain’s certificate which includes cryptographic details & routing information. By including the hostnames cryptography along with routing information, 0-RTT is possible without requiring the client to have visited the domain prior. This is a unique advantage over TLS 1.3 in that 0-RTT is available by default where as in TLS 1.3 one would need to have visited the site prior. Before clients connect to a website they must first query the DIS with a human-readable hostname. The DIS has centralized servers and a decentralized network to provide clients with the fastest possible way to access domain certificates. 

The DIS acts as another layer of defence from malicious certificate related attacks. When invalid certificates are used to request information from the DIS to go to a service the DIS simply denys returning a response.

The decentralized nodes providing domain certificates have a chance to earn Viat through their services. This functionality will be covered in-depth with the Viat white paper.

![DIS](https://sentivate.com/wp-content/uploads/2018/09/SentivateInfographicDIS.png)

### DOMAINS
###### HUMAN READABLE HOSTNAMES

Domains on Sentivate have full extension names and can have single full names for trademarked entities. The domain rules and regulations are designed to organize the web, free up domain names for new companies, protect trademarks, limit malicious activity, and make extensions more descriptive.

For example, one can navigate to Amazon by simply typing Amazon into the Sentivate browser. Domain rules are stricter on the Sentivate network. Domain squatting is entirely disallowed, there is a use it or lose it policy. Domain content or service must be relevant to the domain extension. For example, Amazon's store must use the store domain extension, "Amazon.store". There are shorthand domain extensions available for certain domains. For example, Amazon's company website must utilize the company extension, Amazon.company or the shorthand variant Amazon.com. Bitcoin, Ethereum, and Litecoin are cryptocurrencies and sites dedicated to them must use the cryptocurrency extension. However, a news site related to say bitcoin must use the .news and or .blog extension. Any domain that may have random and or arbitrary content must use the .abstract extension.

## UNIVERSAL IDENTITY SYSTEM

### IDENTITY CERTIFICATES
###### EPHEMERAL & MASTER KEY PAIRS

Identity certificates, (IC), are documents which provide cryptographic details that represent you on the network and are signed by a Identity Registrar. An identity certificate has two cryptographic key pairs: Master and Ephemeral. A master key pair is used specifically for signing ephemeral certificates and is the core identifying key pair. Ephemeral key pairs can be replaced at the owner's discretion. Identity certificates cryptographically authenticate & authorize clients on the network.

Ephemeral Certificates, (EC), are a sub-certificate to the Master Certificate. EC's act as profiles which are used to access user defined services. For example, wallet certificate, banking certificate, general web browsing certificate or for every service. However, one can choose to utilize one single ephemeral certificate for all services. ECs are used for the key exchange process which sets up a bi-directional UDSP connection between the origin and host.

Users can instantly signup, login, and purchase an item with their identity certificate. Servers require a client certificate upon connection to establish a successful UDSP handshake.

Identity certificates form the basis for a decentralized reputation system, which can publicly record good & bad behavior associated with specific certificates. A honeypot can be used to block known bad actors from accessing a service further securing the network.

Identity certificates can be linked to real world identities and assets. Making Sentivate an ideal platform for secure, private, and verifiable voting in elections. Stores and companies can have verified ICs which allow users to directly pay or donate through Viat.

### IDENTITY REGISTRAR
###### VALIDATE AND SIGN

The Identity Registrar, (IR), is a service which signs certificates & is the first layer of protection for the network. The IR protects the network by filtering faulty certificates, stopping Sybil attacks, and nefarious actors. The Identity Registrar ensures malicious certificates aren’t signed which allows services to efficiently deny their connection attempts. False signatures can be denied by the DIS and therefore potentially protect a service and save some of its resources before hand. 

A decentralized network and acyclic blockchain will be leveraged to help validate newly submitted certificates for signing. If the certificated is successfully vetted by the network the IR signs the certificate. Then it can be successfully used by services and the DIS. During the initial handshake, the first packet contains the certificates required to establish a UDSP stream. If signatures are successfully validated the rest of the handshake process continues else it fails.

Active certificates will continually be updated and signed. When a certificate is re-signed, another field is added to the certificate which shows the elapsed time since the previous signing of the certificate. This provides services with an extra layer of trust for certain certificates. 

## DEVELOPMENT

 

### hApps
###### HYBRID UNIVERSAL WEB APPS

Hybrid apps are self-constructing, streaming single-page-applications. Hybrid apps are built using reactive, dynamic, and modular development methodologies. hApps have all the benefits of centralized & decentralized networks ensuring the highest scalability potential.

hApps’ assets are contained in their own file and are streamed to the client on an as needed basis. hApps are streamed and built over time much like a bridge building itself as you walk across. Only one initial page load takes place and thereafter pages are dynamically built as needed similar to Single-page-apps. Only exactly when the client needs the resource is when it will be fetched and delivered.

Sentivate’s components allow for highly modular asset streaming. For example, components can share the same CSS or HTML assets which ensures shared assets are only downloaded once and the duplicate code is never sent over the wire. Server loads and bandwidth is drastically decreased with this methodology as now the client is only pulling exactly what is needed.

Hybrid Apps can utilize an opt-in decentralized P2P CDN for assets in addition to the destination service. Making use of a Hybrid Content Delivery Network means that hybrid apps have high availability, scalability, and more bandwidth.

hApps validate, authenticate, and authorize clients automatically during the initial connection handshake. hApps backends can store and reference clients by their public key or full certificates. Think of it as oAuth for the entire Internet. Services no longer need to worry about hashing, storing, and or encrypting passwords. Clients can quickly login on the click of a button or automatically by simply connecting to the service. Users no longer need to remember or create complex passwords as using their keypair is more secure and easier to use. If services do not require you to have a username they can simply rely on your public key as your identifying name. This means that for some services users don't have to create a username and password during the registration process.

## VIAT

### NATIVE CRYPTOCURRENCY
Viat is the native cryptocurrency on the Sentivate Network. Viat has a hybrid blockchain. Viat’s core systems are decentralized focused but enhanced by centralized components (the opposite of Sentivate’s Web). Viat is designed to be fast, secure, and have some of the lowest transaction fees available. Viat’s centralized portions can process instant transactions, provide wallet security, and alleviate network congestion when the decentralized network is under heavy load. However, these centralized features are opt-in only allowing users to forge their own path.


### MINING 
Viat has a dynamic proof of work which can be mined two ways. Direct mining is the main method, which will be explained in the Viat white paper, & the second method is through the use of packet puzzles in UDSP. Packet puzzles allow for passive mining of Viat while browsing the Universal Web. However, it’s not enabled by default. The situations which arise that enable packet puzzles are: upon connection handshake, connection liveliness check, DDoS protection, congestion control, and or the service chooses to enable it for their own reasons. It is up to the service to enable packet puzzles. This ensures that there is no need for constant mining in the background and gives real purpose to the mining process. Otherwise, it would be on all the time sucking up resources & eating into battery life.
 

### INTEROPERABILITY 
Identity & Domain certificates also double as Viat wallet keys. This allows users to not only instantly sign into a service during a connection handshake, but also provide a way to purchase goods from services, tip sites, and or refund clients. Viat is an integral part of the full functionality of the Universal Web without it only part of the picture is there.
