
# ii. Hafta Ödevleri

# 1. Repomuza ekleyebileceğimiz lisanlar ve aralarındaki farklar nelerdir? 

 Öncelikle yazılım alanında verilen lisanslar ortaya çıkarılmış açık kaynaklı bir yazılım ürününün kullanımı, geliştirilmesi, yeniden yapılandırılması, değiştirilmesi ve alıntı yapılabilmesi konularında yetkili makamları ve sınırları belirleyen telif hakkı olarak görülebilir. Peki bu temel lisanlar ve aralarındaki farklar nelerdir ?
 - #### MIT : 
 >Kullanılan en yaygın lisans türlerinden biri olmakla birlikte 1988 yılında MIT tarafından yayınlandığı için adında MIT geçer. Bu lisansla birlikte yazılıma ait kaynak kodu veya derlenmiş yazılımı dilediğiniz gibi değiştirebilir, yayabilir, kullanabilirsiniz. Ticari olarak kullanım durumu da söz konusudur. Yazılımı geliştirenleri de özgür hale getirdiği için bir sorunla karşılaşılması halinde geliştiriciler için herhangi bir yükümlülük söz konusu olmaz. Bunun yanında MIT ile lisanslanmış bir yazılımı kullandığınızda, o yazılıma referans verilmesi gerekmektedir. En özgür yazılım lisanslarından biri olarak görülür.
 
 - #### Apache Licence : 
 > Lisans, açık kaynak kodlu yazılım geliştirilmesi için kaynak kodlarının kullanımına izin vermektedir. Apache lisansı, MIT lisansı kadar özgür olmasının yanında bu lisansa ait ürünlerin lisanslarını da oluşturduğunuz dağıtıma eklemeniz gerekmektedir. Apache Lisansı yalnızca alıcıyı bilgilendirme amaçlı olarak Apache lisans kodlarının kullanıldığına dair bir uyarının bulundurulmasını zorunlu tutmaktadır. Yeniden dağıtılan yazılım paketlerinde bulunması gereken iki dosya:
LİSANS - kendi lisansının bir kopyası.
UYARI - Geliştiricileriyle birlikte lisanslanmış kütüphanelerin adlarını barındıran bir "uyarı" belgesi.

>Lisanslanmış her belgede, yeniden dağıtım kodlarının barındırdığı tüm özgün telif hakkı ve patent uyarıları korunmalı ve her lisanslı dosyada, bildiri değişiklikleri, değişiklik yapıldığına dair uyarı ile dosyaya eklenmelidir.


- #### GPL :
> GPL ya da GNU ( General Public Licence ), bu lisans ile  yazılım kaynak kodlarına erişebilirsiniz. Fakat GPL ile lisanslanmış bir çalışmayı kullanmanız ve dağıtmanız durumunda sizin yayınladığınız çalışma da GPL lisansına sahip olmalı ve yazılımın kaynak kodlarını içermelidir. Eğer yayınlayıcı kendi kaynak kodları kullanarak başka kişilerin bir ürün oluşturup bunun üzerinde kazanç sağlamasında sorun görüyor ise bu lisans türünü kullanması önerilmektedir. 
> Apache Lisansı ile farkı yazılımların değiştirilmiş sürümlerinin aynı lisansı kullanarak ya da özgür-açık kaynak kodlu yazılım olacak şekilde dağıtılması koşulunu barındırmasıdır.

- #### BSD :
> BSD (Berkeley Software Distribution) lisansı ile MIT lisansının benzer yönleri kullanım izinleri, yeniden dağıtıma izin vermeleri, değişiklikle yeniden dağıtıma izin vermeleri, telif hakkı bildirimini ve garanti sorumluluk reddini saklama hükmü olarak söylenebilir. Yalnız BSD lisansı MIT lisansının aksine birleştirme, yayınlama, alt lisanslama ve satış konularında farklı sınırlara sahiptir. 

# 2. Merge - Squash - Rebase arasındaki farklar nelerdir?
Bu soruyu yanıtlamak için öncelikle merge kavramını anlamalıyız. Merge kısaca branch üzerinde yaptığımız değişiklikleri master branch’i üzerinde birleştirme işlemidir. Merge işlemini yapabilmeniz için repository üzerinde yetkiniz olması gerekmektedir.
**Feature branch** uygulamamızın gelecek versiyonunda eklemeyi plandığımız özellikleri geliştiriğimiz **branch** modelidir. Değişiklikler yapıldıktan sonra feature branch ve master branch merge işlemi ile birleştirilir. 
 
   ![ ](https://miro.medium.com/max/414/1*VtTGNo_autoynCRY0QxxOQ.png)


1. Merge Commits
	>Merge commits ile feature branch üzerindeki bütün değişimler master branche taşınır ve master branch üzerinde toplanarak birleşirler.
	<img src="https://docs.github.com/assets/images/help/pull_requests/standard-merge-commit-diagram.png" width="65%">
	
2. Squash and Merge 
	>Squash ve Merge seçeneği seçildiğinde pull request içinde yapılan değişiklikler sıkıştırılarak kabul edilirler. Devam eden commitler feature branch içinde geliştirme için kullanılırken Github repository geçmişinde olmak zorunda değillerdir. Böylece repository üzerinde daha yalın bir görüntü oluşur. 
	<img src="https://docs.github.com/assets/images/help/pull_requests/commit-squashing-diagram.png" width="65%">
		

3. Rebase and Merge
	>Rebase and Merge seçeneğinde head branch kısmından gelen bütün commitler ayrı ayrı şekilde main branch kısmına eklenirler. Bu seçenek yeniden tabanlama ve düzeltmeler için kolaylık sağlayacaktır. 

# 3. Agile - Scrum - Kanban kavramlarını araştırınız.
- #### Agile nedir ?
>Agile çalışma yapısı sürekli değişen ve gelişen dünyayla birlikte iş süreçlerini sürdürebilmek için ortaya çıkmış bir çalışma modelidir. Bu yaklaşımla birlikte waterfall tekniğinin doğrusal yapısında çıkılır. Agile yazılım geliştirme modelinde de kaynakların ve süreçlerin ileriye dönük ve fırsatlara açık şekilde yapılması temeldir. Uzun vadeli planlardan daha çok kısa dönem planlamaları esastır. Sık aralıklarla parça parça yazılım teslimatını ve değişikliği teşvik eden bir yazılım geliştirme modeli.
>Agile yani çevik çalışma modeline neden ihtiyaç duyulduğu V(Volatility) - U(Uncertainty) - C(Complexity) - A(Ambiguity) kısacası VUCA sebepleri ile açıklanabilir.
>- Volatility, bize hayattaki her unsurun değişim içerisinde olduğunu, bugün çok değerli olanın yarın düşüş yaşayabileceği ve bu durum karşısında kontrolün yitirilmemesi gerektiğini açıklar.
>- Uncertainty, sürekli gerçekleşen bu değişimlerle birlikle belirsizliklerin oluşmaması veya ortadan kalkması için hızlı şekilde aksiyon alabilmek gerektiğini açıklıyor.
>- Complexity, bir durum içerisinde birbiri içine geçmiş sebep sonuç ilişkileri olabileceğini ve bunların durumu karmaşık hale getiriyor olmasına rağmen sonuçta çıkarılan ürünün ileride de gelişime açık olması gerektiğini bize aktarır.
>- Ambiguity, kimi sorunun çözüm kaynaklarının artmasıyla daha belirsiz hale gelebileceği ve bu noktada var olan daha önce denenmiş tecrübelerden de yararlanılması gerektiğini bize anlatır.

>Agile yapısına ait 4 manifesto bulunmaktadır.
 1. İş süreçleri ve araçlardan ziyade bireyler ve bireyler arasındaki etkileşim değerlidir.
 2. Kapsamlı bir dokümantasyon sürecinden ziyade, çalışan bir yazılım ortaya koymak daha önemlidir.
 3. Müşteri ile işbirliği yapmak, sözleşme görüşmelerinden daha önemlidir.
 4. Değişime cevap vermek, mevcut planı izlemekten daha önemlidir.
>
- #### Scrum nedir ?
> Agile manifestosu üzerine “İnsanların mümkün olan en yüksek değere sahip ürünleri üretken ve yaratıcı bir şekilde geliştirirken, karmaşık ve adaptasyona açık sorunları ele alabildikleri bir çerçeve” olan scrum, agile proje yönetme metodolojilerinden biri olarak ortaya çıktı. Yazılım süreçlerinin detaylı ve ihtiyaca göre ortaya çıkan gereksinimlere göre esnek olabilen bir çözüm yönetimidir.
> Scrum ile hızla değişen ihtiyaçlara cevap verebilmek adına, haftalık çalışma planlamaları sprint adı verilen çalışma süreleri içinde gerçekleştirilir. Planlama, süreç iyileştirmeleri ve teslim için farklı ritimlere farklı sprintlere sahip olabilir. İş maddeleri bir Sprint içinde tamamlanacak küçük parçalara bölünmelidir. Devam eden bir Sprinte yeni işler eklenemez. Önceliklendirilmiş bir iş listesi zorunludur. İş geliştirilirken kısa aralıklarla ulaşılabilecek hedefler konulur. Böylece takım hedefe her ulaşmaya çalıştığında deney yapabilir ve önceki deneylerden çıkardığı sonuçlar ile gelecekteki deneylerde daha iyi sonuçlar elde etmek için iyileştirmelerde bulunabilir. Amaç bir ritim yakalamak ve olabildiğince bu ritmi iyileştirerek ilerlemektir. Özetle scrum yapısı için sayılabilecek 3 ana başlık vardır. Şeffaflık, gözetleme ve adaptasyon. 

- #### Kanban nedir ?
>  Kanban, tam zamanında üretim ortamında malzeme hareketlerinin kontrolü amacıyla kullanılan bir çizelgeleme yaklaşımıdır. Bu metodolojide temelde 4 ana düşünceden yola çıkılmıştır. İş akışını görselleştirme, working in progress limitlendirme, lead time yani teslim süresi ölçümü ve sürekli iyileştirme. Kanban, tam zamanında üretim ortamında malzeme hareketlerinin kontrolü amacıyla kullanılan bir çizelgeleme yaklaşımıdır. Kapasite uygun olduğu sürece yeni işler eklenebilir. İşler bir akış mantığı içinde geliştirilir. Akışta bir dar boğaz tespit edildiğinde bu dar boğaza karşı aksiyon alınır ve tekrarlamaması için iyileştirmeler yapılır. Kısa vadelerde belirlenen hedefler yoktur. Geliştirme sürekli olarak devam eder. İş sürekli olarak akar. Amaç işin pürüzsüz bir şekilde sürekli olarak akışını sağlamaktır.

# 4. Github Flow'un alternatifleri nelerdir? Artılarını ve eksilerini karşılaştırınız.
>Github flow düzenli şekilde gelişen ve değişen projeleri ve takımları destekleyen branch-base yapısına sahip bir iş akışı olarak tanımlanabilir.
> Github flowa ait ilerleyiş ilk olarak branch oluşturulması ile başlar. Branch size çalışmak yeni fikirler denemek için yeni bir alan sağlar. Ardından bu branch üzerinde yapacağınız değişiklikleri, geliştirmeleri ve düzeltmeleri commitler halinde branche eklemeniz beklenir. Devamında pull request açarak bu değişimleri herkesin görebileceği ve tartışabileceği şekilde ortaya sunmanız gerekir. Pull request açmak gelişimin her noktasında gerçekleştirilebilir. Bu pull requestler ile geliştiridiğiniz ürünün talepleri karşılayıp karşılamadığını, nerelerde eksik ya da fazla noktalar olduğunu projeyle ilgilenenler ile tartışarak geliştirilebilir. Deploy ile projenizi yaygınlaştırmak ve testlere tabi tutmak için merge işleminden hemen önce gerçekleştirebilirsiniz. Ve son olarak merge işlemi ile oluşturduğunu branchi  main branch e ekleyerek projeyi sunabilirsiniz.


>Github flow içerisinde bir çok prosedür barındırmasına rağmen öğrenmesi oldukça kolay adımlar bütünüdür. Bununla birlikte alternatif olarak Git-flow ya da Gitlab-flow tercih edilebilir. Eğer ürününüz birden fazla platformda çalışacaksa tercihiniz hepsinin gelişimlerini birlikte yürütmek için Git-flow olmalıdır. Fakat eğer ürününüz tek bir platformda karmaşık yapıya sahip ve çok kitleye hitap edecek bir ürün ise pre-production adımları ile test etmenizi kolaylaştıracak olan Gitlab-flow tercih edilmelidir. Bunların yanısıra eğer ürününüz tek sürüm üzerinde daha az karmaşık bir yapıda ilerliyor ise Github-flow tercih edilmelidir.

# 5. Gang of Four (GOF) araştırınız.

>Gang of Four Erich Gamma, Richard Helm, Ralph Johnson ve John Vlissides isimlerinin birlikte oluşturduğu design pattern kitabından yola çıkılarak ortaya çıkmış bir isimdir. Tasarım desenleri yazılım geliştiricilerin zaman içerisinde deneme/yanılma ve  tecrübelerinin sonucunda ortaya çıkmış yazılım geliştirme teknikleridir. Bu desenlerin ortak özellikleri tekrar eden bir probleme karşı geliştirilmeleri, tekrar kullanılabilmeleri, problem çözümü için yeniden en temelden uğraştırmamalarıdır. Desenleri oluşturan belirli kurallar ortak bir platform oluşturup problemleri çözmek, yazılım geliştirme süreçlerini basitleştirmek ve kompleks sistemlerin önüne geçmek amacını taşırlar. Tasarım Desenleri; **Creational, Structural ve Behavioral** olmak üzere 3 başlığa ayrılır.



# 6. Interface ve Abstract sınıflar arasındaki farklar nelerdir?
> Abstract nesne yönelimli programlamadaki önemli kavramlardan biri olarak karşımıza çıkar. Sistemin detaylarını gizleyerek yalnızca işlevlere odaklanmayı sağlayan bir unsurdur. Bu işlem Abstract ve Interface sınıflar aracılığıyla gerçekleştirilir. 

> Abstract sınıflar sınıf hiyerarşisinde genellikle base class tanımlamak için kullanılan ve soyutlama yeteneği kazandıran sınıflardır. Ortak özellikleri olan nesneleri bir çatı altında toplamak için kullanılırlar. Bir sınıfı abstract yapmak için **abstract** keywordünü kullanırız. 
- Abstract sınıflar en az bir tane abstract metod bulundurması bir best practice’tir.
- Abstract sınıftan kalıtım almak için de “**extends**” kullanılır. 
- Abstract class önüne  **virtual** yazılmaz çünkü default, sanal, olarak gelirler. 
- Abstract class, **is-a** ilişkileriyle kullanılırlar. 

>Interface sınıfların OOP yani nesne yönelimli programlamadaki yeri metot ve property listesi olarak karşımıza çıkar. Interface’leri tanımlarken **interface** keywordünü kullanırız. İçerisinde sadece kendisinden türeyecek olan sınıfların içini dolduracağı metod tanımlarının bulunduğu ve soyutlama yapmamıza olanak sağlayan bir yapıdır. Tanımladığımız yapının interface olduğunu belirtmek için isminin önüne I harfini getirmek bir best-practice olacaktır. 
- Interface içerisinde yalnıza metot tanımları bulunur. İçerisine kod parçacığı yazılmaz. 
-Interface başka bir interfaceden inherit olabilir. 
- Interfaceler genelde  **can-do**  ilişkisine göre çalışır. 
- “**new**” ile oluşturulamaz.
-   Bir sınıf birden fazla interface implement edebilir.
-   Interface içerisinde özellik ve metodlarda erişim belirleyiciler kullanılmaz. Her şey  **public** kabul edilir.

<img src="https://miro.medium.com/max/603/0*cTbXWpAKLOEr8hjn.png" width="55%">


#### Kaynaklar 
- https://tr.wikipedia.org/wiki/MIT_Lisans%C4%B1
- https://medium.com/@mehmet.baran/yaz%C4%B1l%C4%B1m-lisans-tipleri-mit-apache-gnu-1397af4d1fbb
- https://tr.wikipedia.org/wiki/Apache_Lisans%C4%B1
- https://resources.whitesourcesoftware.com/blog-whitesource/top-10-apache-license-questions-answered
- https://gist.github.com/nicolasdao/a7adda51f2f185e8d2700e1573d8a633
- https://tr.wikipedia.org/wiki/GNU_Genel_Kamu_Lisans%C4%B1
- https://choosealicense.com/licenses/
- https://opensource.stackexchange.com/questions/217/what-are-the-essential-differences-between-the-bsd-and-mit-licences
- https://medium.com/@alianilkocak/temel-git-terimleri-ve-komutlar%C4%B1-6bc62b802baf
- https://medium.com/@mustafazahidefe/git-notlar%C4%B1-5-branch-kavram%C4%B1-d176626711a4
-  https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/about-pull-request-merges
- https://rietta.com/blog/github-merge-types/
- https://stackoverflow.com/questions/2427238/in-git-what-is-the-difference-between-merge-squash-and-rebase#:~:text=Merge%20squash%20merges%20a%20tree,parent%20commit
- https://medium.com/@aysiinbulus/neler-%C3%B6%C4%9Frendim-agile-57f3c403ae82
- http://www.yilmazcihan.com/scrum-ve-kanban-arasindaki-benzerlikler-ve-farkliliklar/
- https://medium.com/@muhammedsimsek/waterfall-scrum-kanban-ya-da-hi%C3%A7biri-1e93c3b48663
- https://medium.com/@PeopleBox/agile-nedir-scrum-nedir-ba%C5%9Far%C4%B1l%C4%B1-proje-y%C3%B6netimi-y%C3%B6ntemleri-nelerdir-64c4ae723496
- https://guides.github.com/introduction/flow/
- https://stackoverflow.com/questions/18188492/what-are-the-pros-and-cons-of-git-flow-vs-github-flow
- https://stackoverflow.com/questions/39917843/what-is-the-difference-between-github-flow-and-gitlab-flow?rq=1
- https://medium.com/@mbilgil0/abstract-class-vs-interface-bf98133bfadf
- https://medium.com/software-development-turkey/abstract-class-ve-interface-aras%C4%B1ndaki-farklar-nelerdir-3c0a4f956eba
- https://stackoverflow.com/questions/1913098/what-is-the-difference-between-an-interface-and-abstract-class
- https://springframework.guru/gang-of-four-design-patterns/
- https://stackoverflow.com/questions/2056/what-are-mvp-and-mvc-and-what-is-the-difference
- https://medium.com/gokhanyavas/tasar%C4%B1m-desenleri-gof-design-patterns-16e93e54a92d
