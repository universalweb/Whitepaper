# Sentivate Network White Paper - Under Construction

![Logo](https://sentivate.com/wp-content/uploads/brizy/12/assets/images/iW=514&iH=524&oX=0&oY=0&cW=514&cH=524/70e94477b15f379a2717c387bf335188.png)

##### TITLE:  SENTIVATE - The Universal Web. 
#####  ABSTRACT
Sentivate is a hybrid web built to be a viable & realistic replacement for the modern web. The network is designed to go beyond the capabilities that any solely centralized or decentralized network could offer. Sentivate addresses the following issues directly: bandwidth crisis, outdated protocols, broken DNS, lack of accountability, lack of identity, reactive security, Domain rules, and web categorization.

##### FOCUS
This white paper is focused on the core network design that serves as the base network & components for Viat, hApps, and the Universal Web. An additional white paper will be released solely on Viat. All technology is focused on ensuring Sentivateis a revolutionary not an evolutionary replacement, in Internet architecture. 

## INTRODUCTION
##### THE STATE OF THE WORLD WIDE WEB

At present, we find ourselves continuing to utilize a ruinous medium of interconnected communication on a global scale. Humanity’s demands are exponentially increasing of which the World Wide Web simply can’t meet. As we continue to grow, evolve, and venture beyond the solar system, our imperative becomes revolutionizing the technology we depend on.

The current state of the World Wide Web is deprecation. If humanity continues to monkey-patch existing problems the Internet will remain the “wild wild west”. Humanity’s ever-increasing demands will never be met by the current state of the Web. We must start thinking in terms revolutionary not evolutionary. The solution is a complete replacement of contemporary systems, browsers, languages, protocols, and platforms with increased security, efficiency, accountability, trust, identity, capability, and reliability. In order to transition into a new age of information we must replace that which we have become all too comfortable with.


## CRYPTOGRAPHY

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
###### APPLICATION LAYER INTERNET PROTOCOL

##### The Problem
User’s demands have changed and our requirements  of the web have grown. These changes make HTTP a major bottleneck with the heart of the issue being TCP. Large data centers moving copious amounts of data from one end-point to the other have latency and cost issues associated with outdated Internet Architecture. HTTP is especially problematic when users are experiencing low throughput, limited bandwidth, degraded network connectivity, or requiring a near real-time response. The first step in the construction of the Universal Web is to replace HTTP and TCP entirely with UDSP.

##### The Solution
UDSP is a low-latency application layer protocol based on UDP. UDSP is for streaming and or transferring any type of data. UDSP establishes an encrypted bi-directional stream between two clients or one to many clients. All Internet communication on the Sentivate Network utilizes UDSP. When visiting a site on the Sentivate Network UDSP is the protocol used. Specific UDSP client and server modules are required to visit or host a website on the Sentivate Network. UDSP is the backbone and life blood of the Sentivate Network.

UDSP is capable of dynamic reliability on a connection level or on a per-request basis which is agreed upon between the involved parties. UDSP enforces encryption which means all UDSP connections are encrypted by default, no exceptions. UDSP supports IPv6, Multiplexing, and Multihoming. UDSP relies on cryptographic keypairs and XChaCha20 to establish a connection.

UDSP prioritizes the real-time web and Dispersed Computing. Since connections are bi-directional streams and less chatty this makes the network less clogged and ensures low-latency for the livelihood of the connection. UDSP is far less chatty than HTTP and can be programmatically set to adjust it's reliability standards. This makes UDSP a highly useful protocol where high-throughput, low-latency, and high reliability are required. Due to UDSPs programmatically dynamic nature it's efficacious in situations of highly variable and or degraded network connectivity.

UDSP has optional puzzles included in the packets which allow providers and solvers to earn VIAT. Puzzle types vary and thus the puzzles are a Dynamic-Proof-of-Work. The puzzles may be encapsulated or point to data that is required for solving the puzzle. This functionality will be described in the next white paper for VIAT. The puzzles also function as congestion control and a way to limit the potential damages from DDOS attacks. Sentivate turns a typical DDOS attack into profit by the introduction of various puzzle types into packets. When a client solves the served puzzle the client and domain are credited by the network with Viat. If a server is under DDOS attack then the server can dynamically change the reward split up-to 100% for the domain. This ensures the attackers suffer more financial loss and have little to gain. Puzzles ensure that both parties have an incentive to act in good faith. 

![CLIENT CONNECTION](https://sentivate.com/wp-content/uploads/2018/09/DISHyrbid.png)

## UNIVERSAL DOMAIN SYSTEM

### DOMAIN CERTIFICATES
###### ROUTING & CRYPTOGRAPHIC PARAMETERS

Domain certificates provide routing, cryptography, and additional details associated with a hostname. Domain certificates  are signed by 3 or more keypairs: Ephemeral, Master, an authorized Domain Registrar & decentralized nodes on the network. In order to establish a successful handshake the domain certificate is required.

The domain's ephemeral certificate also acts as a wallet which stores funds for any puzzles it distributes to clients. A portion of the mined Viat is sent to the ephemeral certificates wallet address. This topic is covered more in the next white paper for Viat.

### DOMAIN REGISTRAR
###### UPLOAD & SIGN DOMAIN CERTIFICATE

The Domain Registrar, (DR), is used to register a domain and manage a domain's public certificate. The DR validates & signs the public certificates associated with the hostname. The DR then passes the certificate to the Domain Information System which stores the certificate for distribution.


### DOMAIN INFORMATION SYSTEM
###### QUERY DOMAIN ROUTING AND CRYPTOGRAPHY

The Domain Information System, (DIS), returns domain-specific information in the form of a domain certificate from human-readable hostnames. The DIS returns the domain’s certificate which includes cryptographic details & routing information. By including the hostnames cryptography along with routing information, 0-RTT is possible without requiring the client to have visited the domain prior. This is a unique advantage over TLS 1.3 in that 0-RTT is available by default where as in TLS 1.3 one would need to of visited the site prior. Before clients connect to a website they must first query the DIS with a human-readable hostname. The DIS has centralized servers and a decentralized network to provide clients with the fastest possible way to access domain certificates. 

The DIS acts as another layer of defence from malicious certificate related attacks. When invalid certificates are used to request information from the DIS to go to a service the DIS simply denys returning a response.

The decentralized nodes providing domain certificates have a chance to earn Viat through their services. This functionality will be covered in-depth with the Viat white paper.

![DIS](https://sentivate.com/wp-content/uploads/2018/09/SentivateInfographicDIS.png)

### DOMAINS
###### HUMAN READABLE HOSTNAMES

Domains on Sentivate have full extension names and can have single full names for Trademarked entities. The domain rules and regulations are designed to organize the web, free up domain names for new companies, protect trademarks, limit malicious activity, and make extensions more descriptive.

For example, one can navigate to Amazon by simply typing Amazon into the Sentivate browser. Domain rules are stricter on the Sentivate network. Domain squatting is entirely disallowed, there is a use it or lose it policy. Domain content or service must be relevant to the domain extension. For example, Amazon's store must use the store domain extension, "Amazon.store". There are shorthand domain extensions available for certain domains. For example, Amazon's company website must utilize the company extension, Amazon.company or the shorthand variant Amazon.com. Bitcoin, Ethereum, and Litecoin are cryptocurrencies and sites dedicated to them must use the cryptocurrency extension. However, a news site related to say bitcoin must use the news and or blog extension. Any domain that may have random and or arbitrary content must use the abstract extension.

## UNIVERSAL IDENTITY SYSTEM

### IDENTITY CERTIFICATES
###### EPHEMERAL & MASTER KEY PAIRS

Identity certificates, (IC), are documents which provide cryptographic details that represent you on the network and are signed by a Identity Registrar. An identity certificate has two cryptographic key pairs. A master key pair which is used specifically for signing ephemeral certificates and is the core identifying key pair. Ephemeral key pairs can be replaced at the owner's discretion. Identity certificates cryptographically authenticate & authorize clients on the network.

Ephemeral Certificates, (EC), are a sub certificate to the Master Certificate. ECs act as profiles which are used to access user defined services. For example, wallet certificate, banking certificate, general web browsing certificate or for every service. However, one can choose to utilize one single ephemeral certificate for all services. ECs are used for the key exchange process which sets up a bi-directional UDSP connection between the origin and host.

Users can instantly signup, login, and purchase an item with their identity certificate. Servers require a client certificate upon connection to establish a successful UDSP handshake.

Identity certificates form the basis for a decentralized reputation system, which can publicly record good & bad behavior associated with specific certificates. A honeypot can be used to block known bad actors from accessing a service further securing the network.

Identity certificates can be linked to real world identities and assets. Making Sentivate an ideal platform for secure, private, and verifiable voting in elections. Stores and companies can have verified ICs which allow users to directly pay or donate through Viat.

### IDENTITY REGISTRAR
###### VALIDATE AND SIGN

The Identity Registrar, (IR), is a service which signs certificates & is the first layer of protection for the network. The IR protects the network by filtering faulty certificates, stopping Sybil attacks, and nefarious actors. The Identity Registrar ensures malicious certificates aren’t signed which allows services to efficiently deny their connection attempts. False signatures can be denied by the DIS and therefore potentially protect a service and save some of its resources before hand. 

A decentralized network and acyclic blockchain will be leveraged to help validate newly submitted certificates for signing. If the certificated is successfully vetted by the network the IR signs the certificate. Then it can be successfully used by services and the DIS. During the initial handshake, the first packet contains the certificates required to establish a UDSP stream. If signatures are successfully validated the rest of the handshake process continues else it fails.

Active certificates will continually be updated and signed. When a certificate is re-signed another field is added to the certificate which shows the elapsed time since the previous signing of the certificate. This provides services with an extra layer of trust for certain certificates. 

## DEVELOPMENT

### hApps
###### HYBRID UNIVERSAL WEB APPS

Hybrid apps are self-constructing streaming single-page-applications. Hybrid apps are built using reactive, dynamic, and modular development methodologies. hApps have all the benefits of centralized & decentralized networks ensuring the highest scalability potential.

Application’s assets are contained in their own file and are streamed to the client on an as needed basis. hApps are streamed and built over time much like a bridge building itself as you walk across. Only one initial page load takes place and thereafter pages are dynamically built as needed similar to Single-page-apps. Only exactly when the client needs the resource is it fetched and delivered. 

Sentivate’s components allow for highly modular asset streaming. For example, components can share the same CSS or HTML assets which ensures shared assets are only downloaded once and the duplicate code is never sent over the wire. Server loads and bandwidth is drastically decreased with this methodology as now the client is only pulling exactly what is needed.

Hybrid Apps can utilize an opt-in decentralized P2P CDN for assets in addition to the destination service. Making use of a Hybrid Content Delivery Network means that hybrid apps have high availability, scalability, and more bandwidth.

hApps validate, authenticate, and authorize clients automatically during the initial connection handshake. hApps backends can store and reference clients by their public key or full certificates. Think of it as oAuth for the entire Internet. Services no longer need to worry about hashing, storing, and or encrypting passwords. Clients can quickly login on the click of a button or automatically simply by connecting to the service. Users no longer need to remember or create complex passwords as using their keypair is more secure and easier to use. If services do not require you to have a username they can simply rely on your public key as your identifying name. This means that for some services users don't have to create a username and password during the registration process.
