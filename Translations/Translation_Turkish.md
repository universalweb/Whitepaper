
# SENTIVATE WHITEPAPER

![Logo](https://sentivate.com/wp-content/uploads/brizy/3443/assets/images/iW=269&iH=274&oX=0&oY=0&cW=269&cH=274/SNTVTbig.png)

##### BAŞLIK: SENTIVATE- Evrensel Web
#####  ÖZET
Sentivate, günümüz web teknolojisinin yerini almak için geliştirilmiş, uygulanabilir ve gerçekçi bir alternatiftir. Sentivate ağı, merkezi veya merkezi olmayan ağların (centralized/decentralized) herhangi birinin sunabileceklerinin ötesine geçmek için dizayn edilmiş, merkezi odaklı fakat merkezi olmayan bileşenlerle geliştirilmiş karma bir ağdır. Sentivate; bant genişliği, geçerliliğini yitirmiş protokoller, sorunlu DNS, hesap verebilirlik eksikliği, sertifika eksikliği, tepkili güvenlik, alan adı kuralları ve web kategorizasyonu gibi sorunlara doğrudan odaklanmaktadır.

##### ODAK
Bu dökümanda, VIAT’a hizmet edecek temel ağ ve bileşenleri, hApps (hibrit uygulamalar) ve Sentivate evrensel web'i için gerekli çekirdek ağ tasarımı irdelenmiştir. VIAT için ayrıca bir whitepaper yayınlanacaktır. Tüm bu teknolojiler, Sentivate’in günümüz internet mimarisinin yerini alacak evrilmiş bir hali olmasının ötesinde, devrim yaratmasını sağlamaya odaklanmıştır.

## GİRİŞ
##### WWW (DÜNYA ÇAPINDA AĞ) DURUMU

Günümüzde, yıkık dökük, iflas etmek üzere olan, birbirlerine bağlı iletişim araçlarının küresel ölçekte kullanılmaya devam edildiğini görmekteyiz. İnsanlığın talepleri Dünya Çapında Ağ’ın karşılayamayacağı derecede her geçen gün katlanarak artmaktadır. İnsanlık, gelişime, değişime ve güneş sisteminin ötesine geçme girişimine devam ettikçe, bağımlı olduğumuz teknolojide devrim yaratmak bir zorunluluk haline gelmiştir.

Dünya Çapında Ağ’ın şu anki yetersiz durumu kabul edilemezdir. Eğer mevcut sorunlar yama yapılarak çözülmeye devam ederse, internet hep kusurlu olarak kalacaktır. İnsanlığın giderek artan talepleri, Dünya Çapında Ağ’ın varolan durumu tarafından asla karşılanmayacaktır. Bu sebeple mevcut sorunlara devrimsel bir bakış açısıyla yaklaşmaya başlamalıyız. Çözüm; artırılmış güvenlik, hız, verimlilik, hesap verebilirlik, güvenilirlik, kimlik, kapasite ve dayanıklılık ile çağdaş sistemlerin, tarayıcıların, haberleşme yöntemlerinin, protokollerin ve platformların tamamen değiştirilmesidir. Yeni bilgi çağına sağlıklı bir geçiş yapabilmek için, sahip olduğumuz teknolojiyi tümüyle değiştirmek zorundayız.

###### BANT GENİŞLİĞİ SORUNU
[Bant genişliği sınırlıdır, varolan ağlar büyüyen ihtiyaçlarımız için yetersizdir.](https://www.scientificamerican.com/article/the-bandwidth-bottleneck-that-is-throttling-the-internet/) Bu sorunu çözmek için mevcut bileşenlerin yerini alacak modern devrimci teknolojiye ihtiyacımız vardır. Bunu yapmadığımız taktirde, hız şeridi ve verilerin önceliklendirilmesi tek seçeneğimizdir. İnternet servis sağlayıcılarının, tüm internet iletişimine eşit şekilde davranmayacağı ve kullanıcı, içerik, web sitesi, platform, uygulama, ekipman türü veya iletişim yöntemine göre ayrım yapma veya farklı ücret alma korkusu, interneti eğirmek için tek umudumuz olacaktır. IoT (Nesnelerin İnterneti)'nin kaçınılmaz yükselişi, kişi başına düşen cihaz sayısındaki artış, ev başına daha fazla cihaz, kendi kendine sürüş yapan araçlar, araç sigortası mantıksal analizi ve yeni gelişmekte olan ülkeler çevrimiçi olmaya başladıkça, sahip olmadığımız bant genişliği tüketilmeye çalışılacaktır.

###### BEL BAĞLADIĞIMIZ WEB KENDİNİ YEMEKTE
HTTP ve DNS uzun zaman önce, modern taleplerin artacağı düşünülmeksizin inşa edildi. Her geçen gün daha fazla bant genişliği emilmektedir. HTTP, uzun vadeli ölçeklenebilirlik sorunlarını göstermeye devam etmekte ve DNS de güvenilir veya ölçeklenebilir değildir. Eğer WEB'in yarısı DoS-ing'e özgü DNS sunucularından kapatılabiliyorsa, bariz bir mimari problem olduğu aşikardır. HTTP para akışı için mevcut araçtır. Tüm dijital ekonomi HTTP üzerinden taşınır. HTTP veya DNS’e yavaşlama, çok daha yavaş bir küresel ekonomi demektir. DNS ve HTTP doğal olarak bozulmakta, ölçeklenebilirliği zayıf, korkunç derecede yavaş, modern özelliklerden yoksun, bant genişliğini tüketmekte, tüketicilere ve işletmelere milyarlara mal olmaktadır. Bu sorunu çözemezsek, ekonomiye büyük bir darbe ile karşı karşıya kalacağız. Tüm bunları göz önünde bulundurduğumuzda, yakın gelecekte yavaş ağların küresel bir krize yol açacağı açıktır.

1.  [Satışlarda bir saniyelik gecikme Amazon’a 1.6 milyar dolara mal olabilir.](https://www.fastcompany.com/1825005/how-one-second-could-cost-amazon-16-billion-sales_)
2.  [“10 yil önce Amazon, her 100ms'lik gecikmenin satislarda % 1'e mal oldugunu keşfetti”_](https://www.gigaspaces.com/blog/amazon-found-every-100ms-of-latency-cost-them-1-in-sales/)
3.  [“10 yil sonrasının nasıl olacağına dair bir çalışma, web sitesinin yüklenme süresindeki her 100 milisaniyelik bir gecikmenin dönüşüm oranlarini %7 oraninda etkileyebileceğini -bu da satislarda önemli bir düşüştür- Amazon'un saniye ve milisaniye cinsinden gecikmeden bahsetmesinden itibaren %6’dır. Bu durum, e-ticaret başarısı için kullanıcı deneyimlerinin kritik önemde olması sebebiyle, internet perakende satıcıları için işlerin hiç kolay olmadığını göstermektedir. 
”_](https://www.akamai.com/us/en/about/news/press/2017-press/akamai-releases-spring-2017-state-of-online-retail-performance-report.jsp)

###### MERKEZİ OLMAYAN AĞ (WEB 3.0) YETERSİZLİĞİ
Küresel ekonominin yüksek performanslı ve ucuz bir ağ gerektirdiğini biliyoruz. Eğer modern ağın yerini sadece merkezi olmayan bir ağ alırsa, o zaman bant genişliği krizini hızlandıracak ve bizi bir distopya ağına götürecektir. Web 3.0 terimi sihirli bir dünya, devrimci bir fikir veya bir çözüm değil, bir kar elde etme aracıdır. Alım-satım işlemleri nanosaniye mertebesindeki sürelerde gerçekleşir. Küresel ekonominin, alım-satımların saniyeler veya dakikalar gibi blok sürelerinde doğrulanması ve sonrasında ağ üzerinden yayılmasını beklemek için zamanı yoktur. Yeni nesil web, kullanıcılar için daha yavaş ve pahalı olmamalıdır. Web 3.0 daha pahalıya mal olmakta ve “herşey blok zincirinde” gibi şeyler arkasına saklanmaktadırlar ve bir uygulamayı piyasaya sürmenin maliyeti ise çok düşüktür. Gerçek şu ki, ödediğiniz paranın karşılığını vermektedir. Hizmetler yerine kullanıcıya Web 3.0 masrafları yansır, bu ayrıca daha zayıf bir hizmet anlamına gelmektedir. Diğer bir yaygın argüman ise, kullanıcılara verilerini kontrol etme izin vermesidir. Bu bir sorun değildir, buna homomorfik şifreleme denir. Bu konuyu sadece topolojiden ele almak yerine, web'in her alanında yenilik yapmalı ve web servislerimizden daha fazlasını istemeliyiz. İnternetin topoloji problemi, eski teknoloji problemine kıyasla çok azdır. Bu Web 3.0 projeleri aslında web'i değiştirmeye özen gösteriyor olsalardı, asıl konulara odaklanırlardı. **Her iki topolojinin de kendine özgü kullanım durumları vardır, ancak ikisi birlikte kullanıldığında daha önce öngörülememiş ve gittikçe büyüyen bir sorunun çözümü olabilirler.**


## EVRENSEL WEB KRİPTOGRAFİSİ ([SODYUM-NATIVE](https://github.com/sodium-friends/sodium-native))

-  Anahtar İmzalar
    -   Tek parçalı imza: Ed25519
    -   Çok parçalı imza: Ed25519ph
-  Paket Şifreleme
	- Ek Verilerle Kimlik Doğrulaması Yapılmış Şifreleme
    - Mesajı bir anahtarla şifreler, tek bir olay için gizlilik sağlar.
    - Bir kimlik doğrulama etiketi hesaplar. Bu etiket, iletinin yanı sıra isteğe bağlı, gizli olmayan (şifrelenmemiş) verilerin de tahrif edilmediğinden emin olmak için kullanılır.
    - Şifreleme: XChaCha20 akış şifresi
    - Kimlik doğrulama : Poly1305 MAC

- Anahtar değişimi - Paylaşılmış Oturum Gizli Anahtarları
    - BLAKE2B-512
        - AK BLAKE2 bir karma şifreleme işlevidir **MD5, SHA-1, SHA-2 ve SHA-3'ten daha hızlı**, en azından en son standart SHA-3 kadar güvenlidir.
        - NEON etkin ARM'ler dahil 64 bit platformlar için optimize edilmiştir ve 1 ile 64 bayt arasında her boyutta özetler üretir.
    - X25519- Geçici Anahtar Çifti
        - Göndericinin gizli anahtarını ve alıcının genel anahtarını kullanarak gönderenle alıcı arasında paylaşılan bir mahrem bilgiyi hesaplar (veya tersi)

## Hibrit ağ
![Sentivate Hibrit ağ](https://github.com/sentivate/Sentivate-Network-White-Paper/blob/master/images/turkish_1.jpg)

## PROTOKOL

### Evrensel Veri Akışı Protokolü
###### Veri Aktarım Protokolü 

UDSP, UDP tabanlı düşük gecikmeli, gerçek zamanlı, iki yönlü, şifreli ve güvenilir bir Veri Aktarım Protokolüdür.

##### Problem
Giriş bölümünde bahsedildiği gibi: Kullanıcı talepleri her geçen gün değişmekte ve internet gereksinimleri artmaktadır. Bu değişiklikler, HTTP'yi büyük bir tıkanıklık haline getirir. HTTP standardının kendisi ve TCP'nin ikisi de büyük sorunlardır. Çok büyük miktarda veriyi bir uç noktadan diğerine taşıyan büyük veri merkezleri, eski Internet mimarisiyle ilişkili gecikme ve maliyet sorunlarına sahiptir. HTTP, özellikle kullanıcılar düşük veri geçişi, sınırlı bant genişliği, zayıf ağ bağlantısı gibi durumlar yaşadığında veya gerçek zamanlıya yakın bir yanıta gereksinim duyulduğunda, sorunludur.

##### Çözüm
Evrensel Web'in yapımındaki ilk adım, HTTP'yi tamamen UDSP ile değiştirmektir. UDSP, UDP tabanlı düşük gecikmeli, gerçek zamanlı, çift yönlü, şifreli ve güvenilir bir Veri Aktarım Protokolüdür. Evrensel Web'de, tüm iletişim, akış veya herhangi bir veri türünün aktarılması için UDSP kullanılır. Evrensel Web'de bir siteyi ziyaret ederken UDSP, HTTP yerine kullanılan protokoldür. Özel UDSP istemci ve sunucu modülleri, Sentivate Ağındaki bir web sitesini ziyaret etmek veya barındırmak için gereklidir. UDSP, Sentivate Ağının temeli ve can damarıdır.

UDSP, bağlantı düzeyi veya ilgili taraflar arasında kararlaştırılan talep üzerine temelinde dinamik güvenilirliğe sahiptir. UDSP şifrelemeyi zorlar, bu da tüm UDSP bağlantılarının varsayılan olarak şifrelenmiş olduğu, istisnalar olmadığı anlamına gelir. UDSP IPv6, Multiplexing ve Multihoming'i destekler. UDSP, bağlantı kurmak için kriptografik tuş takımlarına ve XChaCha20'ye güvenir.

UDSP, gerçek zamanlı web ve Dağınık Hesaplama(Dispersed Computing)'ya öncelik vermektedir. Bağlantılar, iki yönlü akışlar ve daha az konuşkan olduklarından, bu ağın daha az tıkanmasına neden olur ve bağlantının geçerliliği için düşük gecikme sağlar. UDSP, HTTP'den çok daha az konuşkandır ve kendi güvenilirlik standartlarını belirlemek için programatik olarak ayarlanabilir. Bu, UDSP'yi yüksek verimlilik, düşük gecikme süresi ve yüksek güvenilirliğin gerekli olduğu yerlerde çok kullanışlı bir protokol haline getirir. UDSP'nin programatik olarak dinamik olması nedeniyle, oldukça değişken ve ya da bozulmuş ağ bağlantısı durumlarında etkilidir.

UDSP, paketlerin içinde, sağlayıcıların ve çözücülerin VIAT kazanmasını sağlayan isteğe bağlı yap-bozlara sahiptir. Yap-bozlar değişkenlik gösterebilir ve bu nedenle Dinamik Çalışma Kanıtıdır(Dynamic-Proof-of-Work). Yap-bozlar kapsüllenebilir veya yap-bozu çözmek için gerekli olan verilere işaret edebilir. Bu işlevsellik, VIAT için bir sonraki whitepaper dökümanında açıklanacaktır. Yap-bozlar ayrıca tıkanıklık kontrolü ve DDOS saldırılarından gelebilecek olası zararları sınırlamanın bir yolu olarak da işlev görür. Sentivate, çeşitli yap-boz türlerinin paketlere sokulmasıyla tipik bir DDOS saldırısını kazanç haline getirir. Bir kullanıcı sunulan yap-bozu çözdüğünde, kullanıcı ve alan adı VIAT ile kredilendirilir. Bir sunucu DDOS saldırısı altındaysa, sunucu etki alanı için ödül bölünmesini dinamik olarak% 100'e kadar değiştirebilir. Bu, saldırganların daha fazla finansal zarara uğramasını ve çok az kazanç elde etmesini sağlar. Yap-bozlar, her iki tarafın da iyi niyetli davranmasını teşvik edicidir.

![CLIENT CONNECTION](https://github.com/sentivate/Sentivate-Network-White-Paper/blob/master/images/turkish_2.jpg)

## EVRENSEL ALAN-ADI SİSTEMİ

### ALAN-ADI SERTİFİKALARI
###### YÖNLENDİRME (ROUTING) VE KRİPOGRAFİK PARAMETRELER

Alan-adı sertifikaları, yönlendirme, şifreleme ve bir ana bilgisayar adıyla (hostname) ilişkilendirilmiş ek ayrıntılar sağlar. Alan-adı sertifikaları 3 veya daha fazla anahtar çifti tarafından imzalanır: Ephemeral, Master ve yetkili bir alan-adı kayıtçısı (Domain Registrar). Başarılı bir El Sıkışma oluşturmak için, etki alanı sertifikası ve geçerli bir imza gerekir.

Alan-adının geçici sertifikası, kullanıcılara dağıttığı her yap-boz için fon depolayan bir cüzdan görevi de görür. Madencilikten çıkarılan VIAT'ın bir kısmı geçici sertifika cüzdan adresine gönderilir.

### ALAN-ADI KAYITÇIŞI (DOMAIN REGISTRAR)
###### ALAN-ADI SERTİFİKALARINI KARŞIYA YÜKLEME VE İMZALAMA

Alan-adı kayıtçısı (Domain Registrar), bir alan-adını kaydetmek ve genel sertifikasını yönetmek için kullanılır. Alan-adı kayıtçısı, ana bilgisayar adıyla ilişkilendirilmiş ortak sertifikaları doğrular ve imzalar. Alan-adı kayıtçısı, sertifikayı dağıtım için sertifikayı depolayan Alan-adı Bilgi Sistemine depolar.


### ALAN-ADI BİLGİ SİSTEMİ (DOMAIN INFORMATION SYSTEM)
###### ALAN-ADI YÖNLENDİRME SORGULAMA VE KRİPTOGRAFİ

Alan-adı Bilgi Sistemi, insan tarafından okunabilir ana bilgisayar adlarından bir alan-adı sertifikası biçimindeki alan-adına özgü bilgileri döndürür. Alan-adı Bilgi Sistemi, alan-adının şifreleme ayrıntılarını ve yönlendirme bilgilerini içeren sertifikasını döndürür. Ana bilgisayar adları şifreleme, yönlendirme bilgileriyle birlikte dahil edildiğinde, 0-RTT, kullanıcıdan önceden alanı ziyaret etmesine gerek kalmadan mümkündür. Bu, TLS 1.3'e kıyasla benzersiz bir avantajdır, çünkü 0-RTT varsayılan olarak TLS 1.3'te olduğu gibi siteyi daha önce ziyaret etmiş olmak zorundadır. Kullanıcı bir web sitesine bağlanmadan önce, önce Alan-adı Bilgi Sistemini insan tarafından okunabilen bir ana bilgisayar adıyla sorgulamalıdırlar. Alan-adı Bilgi Sistemi, kullanıcıların alan-adı sertifikalarına en hızlı şekilde erişmelerini sağlamak için merkezi sunucular ve merkezi olmayan bir ağa sahiptir.

Alan-adı Bilgi Sistemi, sertifikaya yapılan kötü niyetli saldırılara karşı başka bir savunma katmanı olarak hareket eder. Alan-adı Bilgi Sistemi'nden bir servise gitmek üzere bilgi istemek için geçersiz sertifikalar kullanıldığında, Alan-adı Bilgi Sistemi yanıt vermeyi reddeder.

Alan-adı sertifikaları sağlayan merkezi olmayan düğümler aracılığıyla VIAT kazanılabilir. Bu işlevsellik VIAT teknik inceleme dökümanında derinlemesine ele alınacaktır.

![DIS](https://github.com/sentivate/Sentivate-Network-White-Paper/blob/master/images/turkish_3.jpg)

### ALAN-ADLARI
###### İNSAN TARAFINDAN OKUNABİLİR ANA BİLGİSAYAR ADLARI

Sentivate üzerindeki alan-adları tam uzantılı adlarına sahiptir ve ticari markalar için tek tam adlara sahip olabilir. Alan-adı kuralları ve düzenlemeleri web'i organize etmek, yeni şirketler için alan adlarını boşa çıkarmak, ticari markaları korumak, kötü amaçlı faaliyetleri sınırlandırmak ve uzantıları daha tanımlayıcı hale getirmek için tasarlanmıştır.

Örneğin, bir kullanıcı Amazon web sitesini açmak istediğinde Sentivate tarayıcısına yalnızca Amazon yazarak gidebilir. Alan adı kuralları, Sentivate ağında daha katıdır. Alan adı ele geçirme işlemine tamamen izin verilmiyor, basitçe ya kullanırsınız ya da alan adını kaybedersiniz. Alan adı içeriği veya hizmeti, alan adı uzantısına uygun olması gerekir. Örneğin; Amazon'un mağazasının "Amazon.store" adlı mağaza alan adı uzantısını kullanması gerekir. Belli alan adları için steno alan adı uzantıları vardır. Örneğin, Amazon’un web sitesi, şirket alan adı uzantısını kullanmalıdır. Amazon.company veya Amazon.com’un steno varyantını kullanmalıdır. Bitcoin, Ethereum ve Litecoin kripto para birimlerine ait web siteleri ise kripto paralar için ayrılmış kripto para birimi uzantısını kullanmalıdırlar. Ancak, bitcoin ile ilgili bir haber yapan siteler ise, .news veya .blog uzantısını kullanmalıdır. Rasgele ve veya rasgele içeriğe sahip olabilecek herhangi bir alan adı .abstract uzantısını kullanmalıdır.

## EVRENSEL KİMLİK SİSTEMİ

### KİMLİK SERTİFİKALARI
###### EPHEMERAL VE MASTER ANAHTAR ÇİFTLERİ

Kimlik sertifikaları, sizi ağda temsil eden ve bir Kimlik Kayıtçısı (Identity Registrar) tarafından imzalanan şifreleme ayrıntılarını sağlayan belgelerdir. Bir kimlik sertifikasının iki şifreleme anahtarı çifti vardır: Master ve Ephemeral. Özel olarak geçici sertifikaları imzalamak için bir ana anahtar çifti kullanılır ve çekirdek tanımlayıcı anahtar çiftidir. Geçici anahtar çiftleri, sahibinin takdirine bağlı olarak değiştirilebilir. Kimlik sertifikaları, ağdaki istemcileri şifreleyerek doğrular ve yetkilendirir.

Geçici sertifikalar (Ephemeral Certificate), ana sertifikaya (Master Certificate) ait bir alt sertifikadır. Geçici sertifikalar, kullanıcı tanımlı servislere erişmek için kullanılan profiller gibi davranır. Örneğin, cüzdan sertifikası, banka işlemleri sertifikası, genel web tarama sertifikası veya tüm servisler için. Ancak, tüm hizmetler için tek bir geçici sertifika da kullanılabilmektedir. Geçici sertifikalar, kaynak ile ana makine arasında iki yönlü bir UDSP bağlantısı kuran anahtar değişim işlemi için kullanılır.

Kullanıcılar, hemen sertifika alabilirler, kimlik sertifikalarıyla kayıt olabilir, giriş yapabilir ve ürün satın alabilirler. Sunucular, başarılı bir UDSP el sıkışması (handshake) oluşturmak için bağlantı sırasında kullanıcı sertifikasını zorunlu tutar.

Kimlik sertifikaları, belirli sertifikalarla ilişkili olarak iyi ve kötü davranışları genel olarak kaydedebilen merkezi olmayan (decentralized) bir itibar sisteminin temelini oluşturur. Bunu cazip kılan şey, kaydedilmiş kötü üne sahip katılımcıların ağ hizmetine erişmelerinin engellemesi, bunun ötesinde ağın daha güvenli hizmet vermesini sağlanmaktır.

Kimlik sertifikaları gerçek dünya kimlikleri ve varlıkları ile bağlantılandırılabilirler. Bu özellik Sentivate'i seçimlerde güvenli, gizli ve doğrulanabilir oylamalar için ideal bir platform haline getirir. Mağazalar ve şirketler de, kullanıcıların doğrudan VIAT ile ödeme veya bağış yapmasına olanak sağlayan doğrulanmış kimlik sertifikalarına sahip olabilirler.

### KİMLİK KAYITÇISI (IDENTITY REGISTRAR)
###### TESCİL VE İMZALAMA

Kimlik kayıtçısı, sertifikaları imzalayan ve ağ için ilk koruma katmanı olan bir hizmettir. Kimlik kayıtçısı, hatalı sertifikaları filtreleyerek, Sybil (bir ağı birden fazla sahte kimlik oluşturarak kontrol etme girişimi) saldırılarını ve kötü niyetli katılımcıları durdurarak ağı koruma görevi görür. Kimlik tescili, kötü amaçlı sertifikaların imzalanmamasını garanti eder, böylece kötü amaçlı bağlantı girişimlerinin engellenmesiyle hizmetin verimini artar. Sahte imzalar alan adı bilgi sistemi (domain information system) tarafından reddedilebilir ve bu nedenle bir hizmeti ve kaynaklarını potansiyel olarak koruyabilir.

Merkezi olmayan (decentralized) bir ağ ve çevrimsel olmayan bir blok zinciri, imzalanmak üzere yeni gönderilen sertifikaların doğrulanmasına yardımcı olmak için kullanılacaktır. Sertifika ağ tarafından başarıyla onaylanırsa, kimlik kayıtçısı (identity registrar) sertifikayı imzalanır. Sonrasında, servisler ve alan adı bilgi sistemi (domain information system) tarafından başarıyla kullanılabilirler. Başlangıçtaki el sıkışma sırasında, ilk paket bir UDSP akışı oluşturmak için gereken sertifikaları içerir. İmzalar başarıyla doğrulanırsa, el sıkışma işleminin geri kalanı devam eder, aksi halde başarısız olur.

Aktif sertifikalar devamlı olarak güncellenecek ve imzalanacaktır. Bir sertifika yeniden imzalandığında sertifikaya, sertifikanın önceki imzalanışından yana geçen süreyi gösteren başka bir alan eklenir. Böylece hizmetlere belirli sertifikalar için ilave bir güven katmanı sağlanmış olur.

## GELİŞTİRME

### hApps
###### HİBRİT EVRENSEL WEB UYGULAMALARI

Hibrit uygulamalar (hApps), mobil uygulamanın tek bir kod ile yazılarak tüm platformlarda (Android,Ios,Windows) çalışan uygulama tipidir. Hibrit uygulamalar duyarlı, dinamik ve modüler gelişim metodolojileri kullanılarak oluşturulmuşlardır. Hibrit uygulamalar, en yüksek ölçeklenebilirlik potansiyelini sağlar, merkezi ve merkezi olmayan ağların tüm avantajlarına sahiptirler.

Hibrit uygulamalar’ın varlıkları kendi dosyalarında bulunur ve müşteriye ihtiyaç duyulduğunda aktarılır. Hibrit uygulamalar zamanla inşa edilir ve akış sağlar, tıpkı üzerinde yürüdükçe kendisini inşa eden bir köprü gibi düşünülebilir. Yalnızca bir ilk sayfa yükleme gerçekleşir ve ardından sayfalar, tek sayfa uygulamalarına benzer şekilde gerektiğinde dinamik olarak oluşturulur. Yalnızca müşterinin ihtiyaç duyduğu zamanda getirilir ve iletilir.

Sentivate’in bileşenleri, oldukça modüler bir varlık akışı sağlar. Örneğin, bileşenler, paylaşılan varlıkların yalnızca bir kez indirilmesini ve yinelenen kodun hiçbir zaman hat üzerinden gönderilmemesini sağlar, tıpkı CSS veya HTML varlıkları gibi. Bu metodoloji ile sunucu yükleri ve bant genişliği önemli ölçüde azalmış olur, çünkü kullanıcı tüm veri yerine sadece tam olarak ihtiyaç duyulan veriyi çekmektedir.

Hibrit uygulamalar, hedef hizmete ek olarak, varlıklar için bir merkezi olmayan (decentralized) P2P (Eşten eşe) CDN (içerik dağıtım ağı)'si kullanabilir. Hibrit İçerik Dağıtım Ağı'nı kullanmak, hibrit uygulamaların yüksek kullanılabilirliğe, ölçeklenebilirliğe ve daha fazla bant genişliğine sahip olduğu anlamına gelir.

Hibrit uygulamalar, ilk bağlantı anlaşması sırasında istemcileri otomatik olarak doğrular ve yetkilendirir. Hibrit uygulama arkayüzleri, istemcileri genel anahtarlarıyla veya tam sertifikalarıyla saklayabilir ve başvuruda bulunabilir. Tüm internet için OAuth (Open Authorization) protokolü olması gibi düşünülebilir. Hizmetlerin artık parolaları toplama, saklama veya şifreleme konusunda endişelenmesine gerek yoktur. Kullanıcılar bir düğmeye tıklayarak veya hızlıca servise bağlayarak otomatik olarak giriş yapabilirler. Tuş takımlarını kullanmak daha güvenli ve kullanımı daha kolay olduğu için kullanıcılar artık karmaşık şifreler hatırlamak veya oluşturmak zorunda değillerdir. Servisler bir kullanıcı adınızın olmasını gerektirmiyorsa, tanımlayıcı adınız olarak genel anahtarınıza güvenebilirler. Bu, bazı hizmetler için kullanıcıların kayıt işlemi sırasında bir kullanıcı adı ve parola oluşturmak zorunda olmadıkları anlamına gelir.

## VIAT

### NATIVE KRİPTO PARA BİRİMİ
VIAT, Sentivate Ağındaki native kripto para birimidir. VIAT hibrit bir blok zincirine sahiptir. Viat’ın çekirdek sistemleri, Sentivate ağının tersine, merkezi olmayan (decentralized) odaklı, ancak merkezi (centralized) bileşenler (Sentivate’in Web’inin tersi) tarafından geliştirilmiştir. VIAT hızlı, güvenli ve mevcut en düşük işlem ücretlerinden birine sahip olacak şekilde tasarlanmıştır. VIAT’ın merkezi bölümleri anlık işlemleri gerçekleştirebilir, cüzdan güvenliği sağlayabilir ve merkezi olmayan ağ ağır yük altındayken ağ tıkanıklığını azaltabilir. Ancak, bu merkezi özellikler yalnızca kullanıcıların kendi yollarını oluşturmasına izin vermek için tercih edilir.

### MADENCİLİK
VIAT dinamik Proof of Work'a sahiptir ve iki şekilde madenciliği yapılabilir. Proof of Work (PoW), Türkçe tabiriyle “işin kanıtı” anlamına gelir (PoW’ün ana hedefi, blok gönderiminden önce yapılması gereken çalışmayı gerektirerek hizmet reddi saldırılarını, yani kısaca DDOS, engellemektir). Doğrudan madencilik, VIAT teknik raporunda açıklanacak olan ana yöntemdir ve ikinci yöntem ise UDSP'de paket yap-bozlarının kullanılmasıdır. Paket yap-bozlar, Evrensel Web’de gezinirken Viat’ın pasif madenciliğinin yapılmasına olanak tanır. Ancak, varsayılan olarak etkin değildir. Paket yap-bozları etkinleştiren durumlar şunlardır: bağlantı el şıkışması, bağlantı canlılığı kontrolü, DDoS koruması, tıkanıklık kontrolü ve / veya hizmet kendi nedenleriyle etkinleştirmeyi seçer. Paket yap-bozları etkinleştirmek hizmete kalmış bir durumdur. Bu, arka planda sürekli madenciliğe gerek kalmamasını ve madencilik sürecinin gerçek amacına uygun olarak verilmesini sağlar. Aksi takdirde, kaynaklar gereksiz yere kullanılacak ve pil ömrünü azaltacaktır.

### BİRLİKTE ÇALIŞABİLİRLİK 
Kimlik ve alan adı sertifikaları ayrıca VIAT cüzdan anahtarları olarak da kullanılır. Bu, kullanıcıların bir bağlantı el sıkışması sırasında yalnızca bir hizmete anında giriş yapmasını sağlamakla kalmaz, aynı zamanda servislerden mal satın alınabilmesini, bahşiş verilebilmesini ve / veya para iadesi yapılmasını sağlar. VIAT, Evrensel Web'in tam işlevselliğinin ayrılmaz bir parçası olup, büyük resmin yalnızca bir parçasıdır.
