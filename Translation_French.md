
# Sentivate Network White Paper

![Logo](https://sentivate.com/wp-content/uploads/brizy/12/assets/images/iW=1200&iH=any/70e94477b15f379a2717c387bf335188.png)

##### SENTIVATE - Le Web universel.
#####  ABSTRAIT
Sentivate est un site Web hybride (centralisé focalisé mais renforcé par des composants décentralisés) conçu pour être un remplacement viable et réaliste du Web moderne. Le réseau est conçu pour aller au-delà des capacités qu’un réseau centralisé ou décentralisé pourrait offrir a lui seul. Sentivate traite directement les problèmes suivants : crise de bande passante, protocoles obsolètes, DNS cassé, Manque de responsabilité, manque d’identité, sécurité réactive, Règles de domaine, et catégorisation du Web.

##### Focaliser
Cette page blanche se focalise sur la conception du réseau de base qui sert le réseau et les composants de base pour Viat, hApps, et le Web universel. Une page blanche supplémentaire sera publiée uniquement sur Viat, Toute la technologie se focalise à assurer que Sentivate soit révolutionnaire, et non pas un remplacement évolutionniste de l'architecture de l’internet moderne.

## INTRODUCTION
##### L'ÉTAT DU WORLD WIDE WEB ( INTERNET )

L'état actuel du Web est obsolète, Si l’humanité continue de régler les problèmes existants, Internet restera le “wild wild west” (Internet sauvage). L’état actuel du Web ne permettra jamais de répondre aux demandes de l’humanité non-stop croissantes. Nous devons commencer à penser en termes révolutionnaires et non évolutifs. La solution est un remplacement complet des systèmes contemporains, navigateurs, langages, protocoles et plates-formes modernes avec une sécurité, une vitesse, une efficacité, une reddition de comptes, une confiance, une identité, des capacités et une fiabilité accrue. Pour entrer dans une nouvelle ère de l'information, nous devons remplacer ça avec quoi nous sommes devenus bien à l'aise.

###### CRISE DE BANDE PASSANTE
[La bande passante est limitée, nos besoins sont en train de développer nos réseaux.](https://www.scientificamerican.com/article/the-bandwidth-bottleneck-that-is-throttling-the-internet/) Pour résoudre ce problème, nous avons besoin d’une technologie révolutionnaire moderne pour remplacer les composants existants. Si nous ne le faisons pas, la voie rapide et la priorisation des données est notre seule option. Toutes ces craintes que les gens ont de l’abrogation de la neutralité du Net seront notre seul espoir de faire tourner le Web.

###### La réseau sur lequel nous nous appuyons se mange
HTTP et DNS ont été construits il y a longtemps sans tenir compte des exigences modernes. De plus en plus de bande passante est aspirée, HTTP continue de montrer ses problèmes d'évolutivité, et DNS n'est pas digne de confiance ni évolutif. Si la moitié du Web peut être fermée à partir de serveurs DNS spécifiques à DoS-ing, il existe un problème évident d'architecture. HTTP est le véhicule actuel de l'argent. L’ensemble de l’économie numérique est transporté via HTTP. Tout ralentissement vers HTTP ou DNS signifie une économie mondiale considérablement plus lente. DNS et HTTP sont intrinsèquement perturbés, ont une faible évolutivité, sont extrêmement lents, manquent de fonctionnalités modernes, consomment de la bande passante et coûtent des milliards aux consommateurs et aux entreprises. Si nous ne résolvons pas ce problème, nous subirons un coup dur pour l’économie. Lorsque vous tenez compte de tous les signes dollar, on se rend vite compte qu’un ralentissement de l’internet est une crise humanitaire mondiale.

1.  [A one second delay could cost Amazon 1.6BB in sales.](https://www.fastcompany.com/1825005/how-one-second-could-cost-amazon-16-billion-sales)
2.  [_“10 years ago, Amazon found that every 100ms of latency cost them 1% in sales”_](https://www.gigaspaces.com/blog/amazon-found-every-100ms-of-latency-cost-them-1-in-sales/)
3.  [_“Fast forward 10 years later, a 2017 Akamai study shows that every 100-millisecond delay in website load time can hurt conversion rates by 7% – that is a significant drop in sales – 6% – from the time when Amazon first talked about latency in seconds and milliseconds. This goes to show that things aren’t getting any easier for online retailers as user experience is becoming critical to e-commerce success.”_](https://www.akamai.com/us/en/about/news/press/2017-press/akamai-releases-spring-2017-state-of-online-retail-performance-report.jsp)

###### LA DÉFAILLANCE  EST LE WEB DÉCENTRALISÉ AKA WEB 3.0
Nous savons que l’économie mondiale a besoin d’un réseau Internet puissant et peu coûteux. Si un Web uniquement décentralisé remplace le Web moderne, alors il accélérerait la crise de bande passante et nous conduire vers un Web dystopique. Le terme Web 3.0 n'est pas un globe magique, une idée révolutionnaire ou une solution; c'est une ponction d'argent. Les échanges se font en nanosecondes. L’économie mondiale n’a pas le temps d’attendre quelques secondes ou quelques minutes avant la fin d’un bloc-temps pour vérifier puis propager à traves le réseau. Un remplacement pour le Web ne devrait pas être plus lent et plus coûteux pour les consommateurs. Le Web 3.0 coûte plus cher et ils aiment se cacher derrière des choses comme si tout se trouve sur la chaîne et que le lancement d’une application soit très peu coûteux. En réalité, vous obtenez le retour de ce que vous avez payé. Web 3.0 compense les coûts pour les utilisateurs plutôt que pour les services, ce qui entraîne également un service plus médiocre. Un autre argument courant est de permettre aux utilisateurs de contrôler leurs données. Ce n'est pas un problème, dites bonjour au cryptage homomorphique.  Au lieu d’aborder ce problème à partir de la topologie, nous devons innover dans tous les aspects du Web et demander davantage à nos services Web. Le problème de topologie du Web est mineur par rapport  à son problème de technologie obsolète. Si ces projets Web 3.0 souhaitaient réellement changer le Web, ils se concentreraient sur les problèmes réels. ** Les deux topologies ont leurs cas d'utilisation, mais les deux ensemble, elles constituent une solution à un problème sans cesse croissant qui n'a pas été vérifié. **

## CRYPTOGRAPHIE UNIVERSELLE SUR LE WEB ([SODIUM-NATIVE](https://github.com/sodium-friends/sodium-native))

- Signatures clés
    - Signature en une partie: Ed25519
    - Signature en plusieurs parties: Ed25519ph
- Cryptage de paquets
    - Cryptage authentifié avec données supplémentaires
    - Crypte un message avec une clé et un nonce pour le garder confidentiel
    - o	Calcule une étiquette d'authentification. Cette balise permet de s’assurer que le message, ainsi que les données facultatives, non confidentielles (non chiffrées), n’ont pas été falsifiées.
    - Cryptage: Cryptage de flux XChaCha20
    - Authentification: Poly1305 MAC

- Échange de clés - Clés secrètes d'une session partagée
    - BLAKE2B-512
        - o	BLAKE2 est une fonction de hachage cryptographique plus rapide que MD5, SHA-1, SHA-2 et SHA-3, tout en offrant au moins la même sécurité que le dernier standard SHA-3.
        - o	Optimisé pour les plates-formes 64 bits, y compris les ARM compatibles avec NEON, et produit des résumés de toute taille entre 1 et 64 octets.
    - X25519 - Paire de clés éphémères
        - Calcule un secret partagé entre l'expéditeur et le destinataire, à l'aide de la clé secrète de l'expéditeur et de la clé publique du destinataire (ou inversement)

## RESEAU HYBRIDE
![Sentivate Hybrid Network](https://sentivate.com/wp-content/uploads/2018/09/hyrbidNetworkTopology.png)

## protocole

### Protocole de flux de données universel
###### Protocole de transport de données

UDSP est un protocole de transport de données basé sur UDP, à temps de latence faible, en temps réel, bidirectionnel, crypté et fiable.

##### Le problème
Comme indiqué dans l’introduction: Les demandes des utilisateurs ont changé et nos exigences du Web ont augmenté. Ces modifications font de HTTP un goulot d'étranglement majeur. La norme HTTP elle-même et TCP sont deux problèmes majeurs. Les grands centres de données qui transfèrent une grande quantité de données d'un point à un autre ont des problèmes de latence et de coûts associés à une architecture Internet obsolète. HTTP est particulièrement problématique lorsque les utilisateurs font face à un faible débit, à une bande passante limitée, à une connectivité réseau dégradée ou à une réponse en temps quasi réel.

##### La solution
La première étape de la construction du Web universel consiste à remplacer entièrement HTTP par UDSP. UDSP est un protocole de transportation de données basé sur UDP, à temps de latence faible, en temps réel, bidirectionnel, crypté et fiable. Sur le Web universel, toute communication, diffusion en continu (streaming) ou transfert de tout type de données utilise UDSP. Lors de la visite d'un site sur Universal Web, UDSP est le protocole utilisé à la place de HTTP. Des modules client et serveur UDSP spécifiques sont nécessaires pour visiter ou héberger un site Web sur le réseau Sentivate. UDSP est la base et le sang vital du réseau Sentivate.

UDSP est capable d'une fiabilité dynamique au niveau de la connexion ou à la demande, sur accord des parties concernées. UDSP applique le cryptage, ce qui signifie que toutes les connexions UDSP sont cryptées par défaut, sans exception. UDSP prend en charge IPv6, le multiplexage et le multihébergement. UDSP s'appuie sur des paires de clés cryptographiques et sur XChaCha20 pour établir une connexion.

UDSP donne la priorité au web en temps réel et à l’informatique Dispersée. Étant donné que les connexions sont des flux bidirectionnels et moins bavardes, le réseau est moins encombré et assure une faible latence au moyens de subsistance de la connexion. UDSP est beaucoup moins bavard que HTTP et peut être configuré par programme pour ajuster ses propres normes de fiabilité. Cela fait de l'UDSP un protocole très utile qui requiert un haut débit, une latence réduite et une fiabilité élevée. Grâce à  la nature dynamique du programme UDSP, il est opérationnel dans les situations de connectivité réseau très variable et / ou dégradée.

UDSP regroupe dees énigmes facultatifs inclus dans les paquets permettant aux fournisseurs et aux solveurs de gagner du VIAT. Les énigmes peuvent varier et constituent donc une preuve dynamique du travail. Les énigmes peuvent être encapsulées ou indiquer des données nécessaires à la résolution des énigmes. Cette fonctionnalité sera décrite dans le prochain livre blanc sur VIAT. Les énigmes servent également de contrôle de congestion et de moyen de limiter les dommages potentiels causés par les attaques DDOS. Sentivate transforme une attaque DDOS typique en profit par l’introduction de différents types d’énigmes dans des paquets. Lorsqu'un client résout l’énigme servi, le réseau et le client sont crédités avec Viat. Si un serveur est soumis à une attaque DDOS, il peut modifier de manière dynamique le partage des récompenses jusqu'à 100% pour le domaine. Cela assure que les attaquants subissent davantage de pertes financières et ont peu à gagner. Les énigmes garantissent que les deux parties sont encouragées  à agir de bonne foi. 

![CLIENT CONNECTION](https://sentivate.com/wp-content/uploads/2018/09/DISHyrbid.png)

## SYSTÈME DE DOMAINE UNIVERSEL

### CERTIFICATS DE DOMAINE
###### PARAMETRES DE ROUTAGE ET CRYPTOGRAPHIQUE

Les certificats de domaine fournissent le routage, la cryptographie et des détails supplémentaires associés à un nom d'hôte. Les certificats de domaine sont signés par au moins 3 paires de clés: Ephémère, Master et un registraire de domaine autorisé. Afin d'établir une négociation réussie, le certificat de domaine et une signature valide sont requis.

Le certificat éphémère du domaine agit également comme un portefeuille qui stocke des fonds pour les énigmes distribuées aux clients. Une partie du Viat extrait est envoyée à l'adresse du portefeuille de certificats éphémères.

### REGISTRAIRE DE DOMAINE
###### TÉLÉCHARGER ET SIGNER LES CERTIFICATS DE DOMAINE

Le registraire de domaine (DR) est exploité pour enregistrer un domaine et gérer le certificat public d'un domaine. Le DR valide et signe les certificats publics associés au nom d'hôte. Le DR passe ensuite le certificat au système d'information du domaine qui enregistre le certificat pour la distribution.

### SYSTÈME D'INFORMATION DE DOMAINE
###### CRYPTOGRAPHIE ET RECHERCHE DE DOMAINE DE QUERY

Le système d'information de domaine (DIS) renvoie des informations spécifiques à un domaine sous la forme d'un certificat de domaine à partir de noms d'hôtes lisibles par l'homme. Le DIS renvoie le certificat du domaine qui inclut les détails cryptographiques et les informations de routage. En incluant la cryptographie des noms d'hôte avec les informations de routage, 0-RTT est possible sans exiger que le client ait déjà visité le domaine. Ceci est un avantage unique par rapport à TLS 1.3 en ce sens que 0-RTT est disponible par défaut car, comme dans TLS 1.3, il aurait fallu avoir visité le site auparavant. Avant de se connecter à un site Web, les clients doivent d'abord interroger le DIS avec un nom d'hôte lisible par l'homme. Le DIS dispose de serveurs centralisés et d’un réseau décentralisé pour fournir aux clients le moyen le plus rapide possible d’accéder aux certificats de domaine.

Le DIS constitue une autre couche de défense contre les attaques malveillantes liées aux certificats. Lorsque des certificats non valides sont exploités  pour demander aux informations du DIS d’aboutir à un service, le DIS refuse simplement de renvoyer une réponse.

Les nœuds décentralisés prévoit des certificats de domaine ont une chance de gagner Viat via leurs services. Cette fonctionnalité sera traitée en détail dans la page blanche Viat.

![DIS](https://sentivate.com/wp-content/uploads/2018/09/SentivateInfographicDIS.png)

### DOMAINES
###### Noms de famille lisibles par l'homme

Les domaines sur Sentivate ont une extension entière de noms. Les règles et réglementations de domaine sont élaborées pour protéger l'environnement, protéger les marques commerciales, limiter les activités malveillantes et rendre les extensions plus descriptives.

Par exemple, on peut accéder à Amazon en tapant simplement Amazon dans le navigateur Sentivate. Les règles de domaine sont strictes sur le réseau Sentivate. Le squattage de domaine est totalement interdit, il existe une stratégie d'utilisation ou de perte. Le contenu ou le service du domaine doit être pertinent pour l'extension de domaine. Par exemple, le magasin Amazon doit utiliser l'extension de domaine de magasin "Amazon.store". Des extensions de domaine abrégées sont disponibles pour certains domaines. Par exemple, le site Web de la société Amazon doit être utilisé par la société, Amazon.com ou la variante abrégée Amazon.com. Bitcoin, Ethereum et Litecoin sont des crypto-monnaies et des sites dédiés à l'utilisation de l'extension crypto-monnaie. Cependant, un site d'actualités lié au bitcoin doit utiliser l'extension .news et ou .blog. Tout domaine pouvant être utilisé de manière arbitraire.

## SYSTÈME D'IDENTITÉ UNIVERSELLE

### CERTIFICATS D'IDENTITÉ
###### EPHEMERAL ET PAIRE DES CLÉS PRINCIPALE

Les certificats d’identité (IC) sont des documents qui fournissent des détails cryptographiques vous représentant sur le réseau et sont signés par un registraire d’identité. Un certificat d'identité comporte deux paires de clés cryptographiques: principale et éphémère. Une paire de clés principale est utilisée spécifiquement pour la signature de certificats éphémères et constitue la paire de clés d'identification principale. Les paires de clés éphémères peuvent être remplacées à la discrétion du propriétaire. Les certificats d'identité authentifient et autorisent de manière cryptographique les clients sur le réseau.

Les certificats éphémères (EC) constituent un sous-certificat du certificat principal. Les EC agissent comme des profils servent à accéder aux services définis par l'utilisateur. Par exemple, certificat de portefeuille, certificat bancaire, certificat de navigation générale ou pour chaque service. Cependant, on peut choisir d'utiliser un seul certificat éphémère pour tous les services. Les EC sont utilisés pour le processus d'échange de clés qui établit une connexion UDSP bidirectionnelle entre l'origine et l'hôte.

Les utilisateurs peuvent instantanément s'inscrire, se connecter et acheter un article avec leur certificat d'identité. Les serveurs nécessitent un certificat client lors de la connexion pour établir une négociation UDSP réussie.

Les certificats d'identité constituent la base d'un système de réputation décentralisé, qui peut enregistrer publiquement le bon et le mauvais comportement associé à des certificats spécifiques. Un pot de miel peut être utilisé pour empêcher des acteurs connus d’accéder à un service sécurisant davantage le réseau.

Les certificats d'identité peuvent être liés à des identités et des actifs du monde réel. Faire de Sentivate une plate-forme idéale pour un vote sécurisé, privé et vérifiable lors d'élections. Les magasins et les entreprises peuvent disposer de CI vérifiés qui permettent aux utilisateurs de payer directement ou de faire un don via Viat.

### REGISTRAIRE D'IDENTITÉ
###### VALIDER ET SIGNER

Le registre d’identité (IR) est un service qui signe les certificats et constitue le premier niveau de protection du réseau. L'IR protège le réseau en filtrant les certificats défectueux, en arrêtant les attaques Sybil et en mettant en scène des acteurs néfastes. Identity Registrar s’assure que des certificats malveillants ne sont pas signés, ce qui permet aux services de refuser efficacement leurs tentatives de connexion. Les fausses signatures peuvent être refusées par le DIS et donc potentiellement protéger un service et économiser certaines de ses ressources à l’avance.

Un réseau décentralisé et une blockchain acyclique seront mis à profit pour aider à valider les nouveaux certificats soumis aux fins de signature. Si le certificat est validé avec succès par le réseau, l’IR signe le certificat. Il peut ensuite être utilisé avec succès par les services et le DIS. Au cours de la première prise de contact, le premier paquet contient les certificats requis pour établir un flux UDSP. Si les signatures sont validées, le reste du processus de négociation se poursuit, sinon il échoue.

Les certificats actifs seront continuellement mis à jour et signés. Lorsqu'un certificat est re-signé, un autre champ est ajouté au certificat. Il indique le temps écoulé depuis la signature précédente du certificat. Cela fournit aux services une couche de confiance supplémentaire pour certains certificats.

## DÉVELOPPEMENT


### hApps
###### APPLICATIONS WEB UNIVERSELLES HYBRIDES

Les applications hybrides construisent elles-mêmes et diffusent des applications d'une seule page. Les applications hybrides sont conçues à l'aide de méthodologies de développement réactives, dynamiques et modulaires. Les hApp offrent tous les avantages des réseaux centralisés et décentralisés, assurant ainsi un potentiel d'extensibilité optimal.

Les actifs de hApps sont regroupés  dans leur propre fichier et sont transmis au client au besoin. Les hApps sont diffusés et construits avec le temps, un peu prêt comme un pont qui se construit lorsque vous traversez. Un seul chargement de page initial a lieu et les pages sont ensuite construites dynamiquement selon les besoins, de manière similaire aux applications à page unique. Ce n'est que lorsque le client a besoin de la ressource que sa récupération et sa remise sont effectuées.

Les composants de Sentivate autorisent un flux d'actifs hautement modulaire.. Par exemple, les composants peuvent partager les mêmes ressources CSS ou HTML, ce qui garantit que les ressources partagées ne sont téléchargées qu'une seule fois et que le code dupliqué n'est jamais envoyé par câble. La charge du serveur et la bande passante sont considérablement réduites avec cette méthodologie, car le client ne fait que retirer exactement ce qui est nécessaire.

Les hApps valident, authentifient et autorisent les clients automatiquement lors de l'établissement de la connexion initiale. Les backends hApps peuvent stocker et référencer les clients par leur clé publique ou leurs certificats complets. Pensez-y comme oAuth pour tout l'Internet. Les services n'ont plus besoin de s'inquiéter du hachage, du stockage et du cryptage des mots de passe. Les clients peuvent se connecter rapidement en un clic ou automatiquement en se connectant simplement au service. Les utilisateurs n'ont plus besoin de se souvenir ni de créer des mots de passe complexes, car l'utilisation de leur paire de clés est plus sécurisée et plus facile à utiliser. Si les services ne nécessitent pas de nom d'utilisateur, ils peuvent simplement utiliser votre clé publique comme nom d'identification. Cela signifie que pour certains services, les utilisateurs n'ont pas à créer de nom d'utilisateur et de mot de passe lors de la procédure d'inscription.


## VIAT

### CRYPTOCURRENCE NATIVE
Viat est la crypto-monnaie native sur le réseau Sentivate. Viat a une blockchain hybride. Les systèmes centraux de Viat sont décentralisés mais renforcés par des composants centralisés (le contraire du Web de Sentivate). Viat est conçu pour être rapide, sécurisé et offre des frais de transaction parmi les plus bas du marché. Les parties centralisées de Viat peuvent traiter des transactions instantanées, assurer la sécurité du portefeuille et alléger la congestion du réseau lorsque le réseau décentralisé est soumis à une charge importante. Cependant, ces fonctionnalités centralisées ne permettent que les utilisateurs de créer leur propre chemin.


### EXPLOITATION MINIÈRE
Viat dispose d'une preuve dynamique de travail qui peut être exploitée de deux manières. L'exploitation directe est la méthode principale, qui sera expliquée dans la page blanche de Viat. La seconde méthode consiste à utiliser des énigmes de paquets dans UDSP. L es énigmes de paquets permettent une extraction passive de Viat lors de la navigation sur le Web universel. Cependant, il n’est pas activé par défaut. Les situations qui se produisent et qui activent les énigmes par paquet sont les suivantes: lors de la connexion, du contrôle de l’animation de la connexion, de la protection contre les attaques DDoS, du contrôle de la congestion et / ou du service choisi pour l’activer pour leurs propres raisons. Il appartient au service d'activer les énigmes par paquet. Cela garantit qu’il n’est pas nécessaire de procéder à une exploitation minière constante en arrière-plan et confère une réelle utilité au processus d’extraction. Sinon, il serait toujours temps d’absorber des ressources et de s’alimenter dans la vie de la batterie.
 

### INTEROPERABILITE
Les certificats d'identité et de domaine représentent aussi un  office de clés de portefeuille Viat. Cela autorise les utilisateurs non seulement à se connecter instantanément à un service lors d'une prise de connexion, mais également de fournir un moyen d'acheter des produits auprès de services, de sites de basculement ou de rembourser des clients. Viat fait partie de toutes les fonctionnalités intégrales du Web universel sans elle, seule une partie de l'image est là.
