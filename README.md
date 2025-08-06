Git nedir
2005 yılında ilk sürümü yayınlanan git,2009 yılına kadar linux ile iç içe olan dağıtık versiyon kontrol sistemiydi.2009 yılında GitHubın açık kaynak projeler için ücretsiz bir şekilde hizmet vermesi aynı yıllarda Bitbucket ve GitLabın benzer git servisleri sağlamaya başlaması geniş bir kitleye ulaşmasını sağladı.␣␣ 
dağıtık bir sürüm kontrol sistemidir.␣␣ 
herhangi bir klosör komutlarla yeni bir git dosya deposu haline gelebilir.␣␣ 
depolarda .git uzantısına sahip alt klasörler vardır.bu uzantıya sahip dosyalar güncel sürümleri ve eski sürümleri içerir.␣␣ 
kendi projenizi versiyon kontrolü altına almak istediğiniz de git init komutu ile bunu sağlayabiliriz␣␣ 
Windowsta git bash uygulaması ile yapılır.komutları aşağıda␣␣ 
$ cd proje/klasörünüzün/yolu/␣␣ 
$ git init␣␣ 
Repistory = projenin uzak bir sunucuda depolanması .kısaltılmış hali repo dur␣␣ 
Branch = Ana branch ve yan branch olarak ikye ayrılır.Bu yapı sayesinde ana yapıyı bozmadan yan branchlarla proje geliştirilebilir␣␣ 
Master= Reponun Ana alanı .␣␣ 
Commit = yapılan değişiklikleri saklayıp kaydedilmesine yarar.␣␣ 
Chechout = commitler üzerinden geçiş yapmamızı sağlar.␣␣ 
Fork = Reponun bir araya getirilmesidir.kopya üzerinde değişiklik yapıldıktan sonra ana depoya gönderilmesidir.␣␣ 
git init = bu komut ile proje dizininde git dizini oluşturulur.burada prijenin repo adresi,veriler vb. şeyler bullunur.␣␣ 
git add = eklemek istediğimiz dosyalar o dizine eklenmesini sağlar.␣␣ 
git rm = bir dosyayı dizinimizden kaldırmak için kullanılır.␣␣ 
git commit = yaptığımızdeğişiklikten sonra bu komut ile değişikliliği kaydederiz␣␣ 
git push = commitledğimiz dosyayı uzak sunucudaki repoya gönderir.␣␣ 
git pull = uzak sunucudaki dosyalarda bir değişiklik oluştuysa kendi local proje dosyaları ile birleştirir.␣␣ 
git merge = iki farklı branchı birleştirmeye yarar.␣␣ 
git clone = mevcut bir git reposunun bir kopyasını almak istediğimizde bu komutu kullanırız.␣␣ 


CI/CD NEDİR?␣␣ 
Sürekli entegrasyon ve Sürekli Dağıtım␣␣ 
CI(Sürekli Entegrasyon) = paylaşılan bir depoda kod değişikliklerini otomaik oluşturur,tes eder ve entegre eder.␣␣ 
CD(sürekli teslimat) = kod değişikliklerinde onay için otomatik olarak üretime hazır ortamlara iletir.␣␣ 
sürekli dağıtım (CD) = kod değişikliklerini doğrudan müşterilere otomatik olarak dağıtır.␣␣ 
Bunlar bir araya geldiğinde,Geliştirici ekiplerin manuel görevlerini azaltan otomatik bir sistem olan CI/CD hattı oluşur.␣␣ 
Sistemin tekrar eden sürümleri destekleyecek şekilde tasarlanmalı.␣␣ 
CI/CD kullanım␣␣ 
CI : Build + Test␣␣ 
dotnet restore paketleri çeker␣␣ 
dotnet build : projeyi derler␣␣ 
dotnet test : Unit testleri çalıştırır␣␣ 
CD: Publish + Deploy␣␣ 
dotnet publish : deploy edilecek klasörü hazırlar(Çalıştırabilir hale getirilir.)␣␣ 
Azure Web app'a atılır␣␣ 
Docker image oluşturulur␣␣ 
IIS'e deploy edilir␣␣ 





Azure DevOps␣␣ 
yazılım geliştiren ekipler için tümleşik araçlar sağlayan bulut tabanl bir platformdur␣␣ 
Temel Azure hizmetleri␣␣ 
-Azure Boards␣␣ 
-Azure Pipeline␣␣ 
-Azure Repos␣␣ 
-Azure Test plans␣␣ 
-Azure artifacts␣␣ 
Azure Boards␣␣ 
ekip arasında planlama ,izleme yapmak için kullanılır.birikmiş işler,özel raporlar için panolar oluşturulabilir.Bu panolar özlleştirilebilir ve izleme araçlarıyla anlamlı bilgiler edinebilirsin.␣␣ 
Azure Repos␣␣ 
kullanıcıların kod tabanlarını yönetmelerini sağlayan kod depolarıdır.Git sürüm kontrol sistemlerinide destekleyen bulut tabanlı depolardır.␣␣ 
Azure Pipeline␣␣ 
otomatik oluşturma,test etme ve dağıtım işlemlerini kolaylaştıran CI/CD aracıdır.␣␣ 
Azure Testplans␣␣ 
kullanıcıların test gereksinimlerini yönetebilmek için bulut tabanlı test platformunu entegre edebilemey olanak sağlar.␣␣ 
Azure Artifactss␣␣ 
paketleri oluşturmak, depolamak ve paylaşmak için kullanılan yapıt kitaplığı hizmetidirkullanıcıların tüm özelliklere sahip paket yönetimi işlevlerini CI/CD kanallarına entegre etmelerini sağlar.␣␣ 









SDLC nedir?␣␣ 
Bir yazılım geliştirme sürecindeki tüm faaliyetleri açıklayan kavram bütünüdür.Yüksek kalite ,etkili ve verimli yazılım geliştirmek ve zamanı minimum düzeyde tutmak için bir çerçevedir.Bu çerçeve belli aşamalrdan oluşurve her bir aşama bir sonraki aşamaya ürün bırakır.␣␣ 
AŞAMALAR:␣␣ 
1.ANALİZ␣␣ 
Yazılım geliştirme sürecinin ilk aşaması analizdir.Bu aşamada kullanıcı ihtiyaçları belirlenir ve bunlar nasıl karşılanır düşünülür.␣␣ 
2.PLANLAMA␣␣ 
analiz bittikten sonraplanlama kısmına geçilir.Bu aşamada projenin nasıl ilerleyeceğine dair plan yapılır.Planlama sürecinde hangi programlama dili kullanılıcağı,hangi araçların kullanılacağı ve ne kadar zaman süreceği planlanmaktadır.␣␣ 
3.TASARIM␣␣ 
planlama kısmı bittikten sonra tasarım kısmına geçilir.Bu aşamada arayüzler tasarlanır veya işlevler belirlenir.␣␣ 
4.GELİŞTİRME␣␣ 
Bu aşamada yazılım kodu yazılır.Geliştirme Sürecinde yazılımın kullanıcı ihtiyaçlarına yönelik olduğuna dairemin olunmalıdır.␣␣ 
5.TEST ETME␣␣ 
Bu aşamada ,yazılımın doğru çalışıp çalışmadığı kontrol edilir.hata olup olmadığı ,güvenliği,performansı gibi faktörler dikkate alınır.␣␣ 
AGİLE metodolojisi␣␣ 
Yazılım geliştirme projelerinde katı ve sabit planlar yerine , gereksinimlere göre değişen ortama hızlı uyum sağlamayı hedefleyen br metodolojidir.Proje küçük parçalara bölünerek her parça üzerinde ayrı ayrı çalışılır.takım çalışmasına teşvik eder ve ekip üyeleri arasında sürekli bir iletişim olur␣␣ 
SCRUM nedir?␣␣ 
Agile metodolojisinin parçası olan bir çerçevedir.bu çerçeve belirli roller ve yapılar etrafında organize edilir.kısa dögüler halinde çalışılır ve bu döngülere sprint adı verilir.her sprint sonunda hedeflenen ürün veya iş ortaya çıkar.␣␣ 
Scrum takımında Roller␣␣ 
1.Scrum Master : takımın kurallara uygun çalışmasını sağlar ve engelleri kaldırır.işbirliğini teşvik eder.Motivasyonu yüksek tutarak projenin hedeflerine ulaşmasını sağlar.␣␣ 
2.Product Owner:müşteri gereksinimini belirler.Müşteriden gelen feedbackleri toplar ve buna göre öncelikleri belirler.␣␣ 
3.Geliştirme Takımı :yazılım geliştiren ve teslim eden ekip üyelerinde oluşur.belirlenen hedeflere ulaşmak için birlikte çalışır ve her sprint sonunda işlevsel bir yazılım parçasını tamamlar.␣␣ 




GitHub Actions nedir?␣␣ 
yazılım geliştirme sürecinde otomatik iş akışları tanımlamak için kullanılan ,Github tarafından sağlanan bir CI/CD sistemidir.␣␣ 
Pipeline(İŞ akışı nedir?)␣␣ 
yazılım geliştirme sürecinde birbirini takip eden otomatik adımlar dizisidir.Github Actions da␣␣ 
pipline ,bir veya birden fazla görev ve bu görevlerin içinde yer alan steps(adımlar) biçiminde yapılandırılır.␣␣ 
3. Yapılandırma Dosyası␣␣ 
GitHub Actions iş akışları, projenin kök dizininde yer alan .github/workflows/ klasörü altında bir YAML dosyası olarak tanımlanır. Bu dosyada, iş akışının hangi olayla tetikleneceği, hangi sistemde çalışacağı ve hangi adımların gerçekleştirileceği belirtilir.␣␣ 
Örnek: Basit Bir "Hello World" Workflow␣␣ 
Bu örnek yapı, her push işlemi gerçekleştiğinde tetiklenir ve basit bir mesajı terminale yazdırır. Örnekte bir adet job ve onun içinde bir adet step yer almaktadır.␣␣ 




.Net Nedir?␣␣ 
.NET'in çeşitli uygulamaları, .NET kodunun Linux, macOS, Windows, iOS, Android ve diğer işletim sistemlerinde çalıştırılmasına izin verir.␣␣ 
.NET Tarihçesi␣␣ 
2000-2007␣␣ 
ilk beta sürümü 2000 yılının sonunda yayınlandı ve 13 Şubat 2002 de ilk sürüm olan .NET 1.0 yayınlandı.temel özelliği web uygulamalarının nesne yönelimli geliştirilmesini destekliyordu.␣␣ 
NET 1.1 (Nisan 2003): Bir dizi geliştirme (örneğin ASP.NET için güvenlik geliştirmeleri), İnternet Protokolü Sürüm 6 desteği ve ODBC içeriyordu.␣␣ 
.NET 2.0 (Kasım 2005): Genel koleksiyonlar, yineleyiciler, ASP.NET için yeni özellikler, geçersiz türler vb. içeriyordu.␣␣ 
.NET 3.0 (Kasım 2006): öne çıkanlar WPF (Windows Presentation Foundation), WCF (Windows Communication Foundation), WWF (Windows Workflow Foundation).␣␣ 
2007␣␣ 
kaynak kodu kullanıma sunuldu.Bu sürüme .NET3.5 adı verildi.bu sürümün temel özellikleri şunlardı:␣␣ 
AJAX desteği,␣␣ 
Dinamik veriler,␣␣ 
LINQ ␣␣ 
ASP.Net MVC␣␣ 
Microsoft, 2014 yılına kadar çerçevenin birkaç versiyonunu daha yayınladı:␣␣ 
.NET 4.0 (Nisan 2010): Yönetilen Genişletilebilirlik Çerçevesi, DLR, görev paralel kütüphanesi, Razor görünüm motoru.␣␣ 
.NET 4.5 (Ağustos 2012): Async desteği, daha iyi ASP.NET desteği, Zip sıkıştırma desteği, geliştirilmiş CLR 4.0␣␣ 
.NET 4.5.1 (Ekim 2013): daha iyi performans ve hata ayıklama, Windows Mağazası uygulama geliştirme için gelişmiş destek.␣␣ 
2014 .NET Core'un başlangıcı␣␣ 
Bu zamana kadar .NET ' in en büyük kusuru windows dışındaki platformlarda çalışamamsıdır.Bu sorunu çözmek için Microsoft 2014 yılında .NET Core duyurdu.␣␣ 
.NET ile neler yapılabilir?␣␣ 
.NET ile kullanarak şu uygulamalar geliştirilebilir:␣␣ 
Windows Uygulamaları,␣␣ 
Windows Phone Uygulamaları,␣␣ 
Web Uygulamaları (ASP.Net),␣␣ 
Oyunlar␣␣ 
Mobil Uygulamalar␣␣ 
Windows Azure ile cloud uygulamaları,␣␣ 
MS Office için eklentiler,␣␣ 
Veri tabanı uygulamaları ␣␣ 
.NET'in avantajları Nelerdir?␣␣ 
Geliştirme Kolaylığı␣␣ 
Zaman Tasarufu␣␣ 
Yüksek performanslı uygulamalar oluşturma␣␣ 
Güvenilirlik␣␣ 
Zengin Kaynak ve kitaplıklar␣␣ 
Topluluk desteği␣␣ 


<img width="554" height="479" alt="image" src="https://github.com/user-attachments/assets/c2a31f66-db2a-49e5-b500-2b2773b17c3a" />





Senkron ve Asenkron Programlama
Senkron Programlama
-İşlemler Sırasıyla yapılır.Bir işlem bitmeden diğer işleme geçilemez.Doğrusal ve anlaşılması kolaydır.Ağır görevlerde işleri yavaşlatabilir ve gecikmelere neden olabilir.
Asenkron Programlama
-Asenkron programlama , birden fazla belgenin aynı anda işlenmesi gibi zaman alan işlemleri gerçekleştirmek içindir.Tarayıcılar buna bir örnek olabilir.
Temel anahtar kavramlar
1.async
bir metodun asenkron olduğunu gösterir. Geri dönüş tipi Task ' dır

public async Task<string> VeriGetirAsync()
{
await Task.Delay(1000); // simülasyon
return "Veri hazır";
}
2.await
asenkron işlemi başlatmaya yarar.sonucu beklerken thread kilitlenemez
3.Task
Sonuç dndüremeyen işlemler için kullanılır.
4. ConfigureAwait
UI thread veya synchronization context gerekmeyen yerlerde performans ve deadlock riski için önemlidir
C#’ta => (Arrow Function) İfadesi
Bu operatör , lambda ifadelerinde ve kısa method tanımlamalarında geçer.
1. Lambda ifadesi
Func<int, int> karesi = x => x * x;
Console.WriteLine(karesi(5)); // 25
2. Kısa method
public int Topla(int a, int b) => a + b;
3. Property
public string Ad => "baba"; // readonly, expression-style property
















dotnet --info çıktısı örneği ve yorumlama

.NET SDK (reflecting any global.json):  Version:   8.0.100  // Şu anda kullanılan SDK sürümünü belirler  Commit:    3d885d3f90  Runtime Environment:  OS Name:     Windows // hangi işletim sistemi üzerinde çalıştığımızı gösterir  OS Version:  10.0.22621 //İşletim sisteminin sürümünü gösterir  OS Platform: Windows  RID:         win10-x64 //Proje hangi sistem için build edileceğini gösterir  Base Path:   C:\Program Files\dotnet\sdk\8.0.100\ //SDK nın kurulu olduğu dosya yolunu gösteri  Host:   Version:      8.0.0   Architecture: x64   Commit:       5678abcd12  .NET SDKs installed:// Makinede kurulu Tüm SDK sürümlerini gösterir   6.0.416 [C:\Program Files\dotnet\sdk]   7.0.306 [C:\Program Files\dotnet\sdk]   8.0.100 [C:\Program Files\dotnet\sdk]  .NET runtimes installed://çalıştırmak için gerekli runtime'ları listeler   Microsoft.AspNetCore.App 6.0.16 [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]   Microsoft.AspNetCore.App 7.0.9  [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]   Microsoft.AspNetCore.App 8.0.0  [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]   Microsoft.NETCore.App 6.0.16    [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]   Microsoft.NETCore.App 7.0.9     [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]   Microsoft.NETCore.App 8.0.0     [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]  Other architectures found: alternatif kurulumları gösterir.   x86   [C:\Program Files (x86)\dotnet\]  Environment variables: Sistemdeki çevre değişkenlerini gösterir.   DOTNET_ROOT = C:\Program Files\dotnet



BackEnd nedir?
Backend ,kullanıcının web sitesinde veya bir uygulamada kullanırken görmediği ama uygulamanın düzgün çalışmasını sağlayan kaynak kodlar ve veritabanından oluşan kısımdır.
Veritabanının ve uygulamanın birbiri ile iletişime geçmesini sağlayan ,sorunsuz çalışmasını sağlayan kodlardan oluşur.
FrontEnd ve BackEnd farkı
bu ikisi arasındaki temel farklar ilgilendikleri alan ve teknolojilerdir.Frontedn Kullanıcın etkileşime girdiği kısımla ilgilenirken,backend daha ço uygulamanın işlemlerinin nasıl gerçekleşeceğiyle ilgili kısımdan sorumludur.

Web Sunucusu nedir?
internet ortamında web sitesinin yayınlanmasından sorumlu olan sunucudur.Hosting işlemini internet protokolü üzerinden yapar.Hosting,Web sitelerinin yayınlanmak için gerekli alanı kiralamasıdır.



API nedir?
İki yazılım projesinin birbirleriyle iletişim kurmasını sağlayan bir nevi anahtardır.
API türleri
-Özel API'ler
Yalnızca kullanılacak olan işletmenin içindeki sistem ve verileri bağlamak için kullanılır.
-Genel API'ler
halka açık,herkesin kullanabileceği API türüdür.
-Çözüm Ortağı API'ler
işletmeler arası yardım sağlamak amaçlı kullanılar API'lerdir.
-Birleşik API'LER
karmaşık sistemler için iki veya daha fazla AOI'yi bir araya getirir.

HTTP nedir?
HTTP ,WWW'in temelini oluşturur.Köprü metni bağlantıları kullanarak web sayfalarını kullanır.Cihazlar arasında bilgi aktarım için kullanılır.İstemcinin sunucuya istekte bulunmasını ve sunucunun bir geri bildirim vermesini sağlar.
HTTP metodları
-GET
Sunucudan veri istemek için kullanılır
GET /search?q=security+engineer HTTP/1.1
Host: google.com
bu ısımda veri URL'nin içine gömülüyor.sunucudan security engineer arama sonuçları isteniyor
-POST
Sunucuya veri göndermek için kullanılır
POST /login HTTP/1.1
Host: example.com
Content-Type: application/json

{
"username": "baba",
"password": "hunter2"
}
Veri burada get'deki gibi URL'de değil body kısmında taşınır.
-PUT
sunucuya bir kaynağı yerleştirmek için kullanılır.
PUT /api/users/123 HTTP/1.1
Content-Type: application/json

{
"id": 123,
"username": "baba",
"email": "baba@cybermail.io"
}
-DELETE
Sunucudaki bir veriyi silmek için kullanılır.
DELETE /api/users/123 HTTP/1.1
bu kodda da id'si 123 olan kullanıcıyı siliyor.
JSON nedir?
JSON bir kod bloğu değildir.Depoları saklamak ve aktarmak için kullanılır.Farklı programlama dilleri arasına rahatlıkla veri değişimi sağlar.Genellikle web uygulamaları ve sunucular arasında veri göndermek için kullanılır.
JSON veri tipleri
-Nesneler
-Diziler
-Dizeler
-Mantıksal değer
-Null
-Sayı
örnek
```
{
"name": "Sergen İlhan Yağlı",
"age": 21,
"city": "Bursa",
"phone": "5511711763",
"email": sergenilhany67@gmail.com"
}
```

REST vs SOAP vs GraphQL
REST http +JSON/XMl kullanırken SOAP XML+WS kullanır GraphQL ise HTTP+JSON kullanır
veri formatları Rest'te JSON veya XML SOAP ta ise sadece XML GraphQL de ise sadece JSON kullanılır.
REST 'te güvenlik HTTPS ,OAuth ,JWT ile sağlanır,SOAP ta ise WS-Security ile,GraphQL'de ise HTTPS ,OAuth ,JWT ile sağlanır.


Dependency Injection Kullanımına Örnek
public interface ILogger
{
void Log(string message);
}
bir interface oluşturuyoruz
public class ConsoleLogger : ILogger
{
public void Log(string message)
{
Console.WriteLine("Log: " + message);
}
}
önceki interface'e bağlı bir sınıf yazıyoruz
public class Game
{
private readonly ILogger _logger;

// DI burada: logger dışarıdan veriliyor
public Game(ILogger logger)
{
_logger = logger;
}

public void Start()
{
_logger.Log("Oyun başladı!");
}
}


Performans için önerilen en az 3 teknik ve açıklamaları
1.AsNoTracking()
EF Core ,default ayar olarak her veriyi takip eder.Ama sadece veriyi okuma işlemi yapacaksan bu çok gereksiz bir yük olur.
bu tekniği kullanırsan sorgulama neredeyse %50 hızlanır ,bellek tüketimi azalır.
2.Caching
Aynı veriyi sürekli sorguluyorsak bu zaman ve kaynak kaybıdır.Caching ile bu durumun önüne geçiyoruz.Bu sayede DB sorgu sayısı azalır.
3.DTO+Select
EF'de bir entity'yi doğrudan çağırırsan tüm alanları çekmiş olursun buda bellekteki yükü arttırır.Bu teknik sayesinde sadece gerekli alanlar çekilir.Ağ trafiğide düşer.


OWASP 10 listesi ve her biri için 1–2 cümlelik açıklamalar
1.Brokjen Access Control
Kullanıcı,yetkisi olmayan alanlara erişebilme durumudur.
2.Cryptographic Failures
Veriler doğru şifrelenemiyor veya hiç şifrelenemme durumudur.
3.Injection
Kullanıcıgirişi doğrudan sorguya eklendiği için sxaldırgan komut enjekte edebilir.
4.Insecure Design
Uygulamanın en baştan beri güvenliğe uygun dizayn edilmemesidir.
5.Security Misconfiguration
Güvenlik ayarlarının eksik,yanlış veya varsayılan bırakılmasıdır.
6.Vulnurable and Outdated Components
Kullanılan kütüphane veya yazılımların eski veya bilinen açıkları içermesidir.
7.Identification and authentication Faailures
Kimlik doğrulama sistemi zayıf olduğunda saldırganların kolayca hesaplara erişebilmesidir
8.Software and Data ıntegrity Failures
uygulama güncellemeleri,kod veya veriler doğrulama yapılmadan çalıştırılması.
9.Security logging and Monitoring Failures
Loglama eksik veya olmadığından saldırı girişimleri tespit edilememesidir.
10.Server-Side Request Forgery
Saldırganın sunucunun farklı adreslere istek göndermesini sağlayabiliyor.

Her SOLID prensibi için kısa örnek
Single responsibility Principle(SRP)
bir sınıfın sadece bir sorumluluğa sahip olması
örn
class ReportGenerator { public void Generate() { } }
class ReportSaver { public void SaveToFile() { } }
Open/Closed Principle(OCP)
sınıfların geliştirmeye açık değişime kapalı olması
örn
interface IDiscount { double GetRate(); }

class RegularDiscount : IDiscount { public double GetRate() => 1.0; }
class PremiumDiscount : IDiscount { public double GetRate() => 0.8; }

class DiscountCalculator
{
public double Calculate(IDiscount discount) => discount.GetRate();
}
Liskov Substitution Principle
türeyen sınıf,ana sınıfın yerine sorunsuz geçebiliyor olmalı
örn
interface IBird { }
interface IFlyingBird : IBird { void Fly(); }

class Sparrow : IFlyingBird { public void Fly() { } }
class Ostrich : IBird { }
Interface Segregation Principle
arayüzler küçük ve öz olmalı,kullanılmayan metotlar içermemeli
örn
interface IWorkable { void Work(); }
interface IEatable { void Eat(); }

class Robot : IWorkable { public void Work() { } }
Dependency Inversion Principle
Üst Sınıflar ,soyutlamalara bağlı kalmalı somut sınıflara değil
örn
interface IMessageService { void Send(); }

class EmailService : IMessageService { public void Send() { } }

class Notification
{
private IMessageService _service;
public Notification(IMessageService service) { _service = service; }
public void Alert() => _service.Send();
}


En az 2 design pattern açıklaması
1.Singleton pattern
Uygulama boyunca instance olmasını istediğin tek bir sınıf için kullanılır.
Amaç:Belleğimde sadece 1 sınıf olsun ve tüm sistem ortak kullansın
2.Strategy pattern
Değişken algoritmaları runtime içinde seçilebilir hale getirir.Örn:İndirim hesaplamaları
Amaç:farklı algoritmalar birbirinin yerini sorunsuz bir şekilde alır.

Clean Code uygulama örnekleri
Anlamlı isimlendirme
Örn
İnt d;
burada tam olarak neyi tanımladığımız belli olmayabilir ama
int arabaModel;
gibi daha açık tanımlama yaparsak değişkenlere daha temiz olur.
Fonksiyonlar kısa ve tek iş yapmalı
void HandleUser()
{
Validate();
Save();
SendEmail();
}
burada fonksiyonlara genel bir tanımlama yapılmış
void HandleUser()
{
ValidateUser();
SaveUser();
SendWelcomeEmail();
}
böyle daha iyi.
Gereksiz yorum satırı ekleme
// kullanıcıya e-posta gönderir
SendEmail();
bunu açıklamak yerine fonksiyon isminden ne olduğunu anlayalım
SendWelcomeEmail();

			

<img width="513" height="365" alt="image" src="https://github.com/user-attachments/assets/7021e8cd-f2cd-4189-aa47-31db9c056503" />

				


Log seviyelerinin açıklamaları
-Debug
geliştime sırasında kullanılan adımlarını tek tek göstermeye yarayan bir log
-ınformation
uygulamanın normal işleyişini bildirir.Önemli olayları loglar.
-Warning
Şüpheli olan durumları bildirir bu durularda sistem çalışmaya devam eder ama ileride sıkıntı çıkarabilir.
-Error
Hata logudur.Sistemde bir şeylerin yanlış veya eksik olduğunu gösterir.


Örnek hata yönetim kodu  açıklaması

public User GetUserById(int id)
{
try
{
// DB'den kullanıcıyı çek
var user = dbContext.Users.First(u => u.Id == id);

// Kullanıcı bulunursa döndür
return user;
}
catch (InvalidOperationException)
{
// Kullanıcı yoksa (First() patlar)
Console.WriteLine($"Hata: ID {id} ile kullanıcı bulunamadı.");
return null;
}
catch (Exception ex)
{
// Beklenmeyen her şeyi burası yakalar
Console.WriteLine("Beklenmeyen hata: " + ex.Message);
return null;
}
finally
{
// Her durumda çalışır (başarılı ya da hata)
Console.WriteLine("GetUserById çalışması tamamlandı.");
}
}
try: Riskli kod kodlar buraya yazılır.
catch : hata oluşursa buraya gelir.birden fazla olabilir bü yüzden tipi önemlidir.
catch(InvalıdOperationException) : First() kullanıcı bulamazsa bu hatayı verir
catch (exception ex) : genelhata yakalama.Özel türler önce yazılır,en sona gelir.
finally: hata olsada olmasada çalışır.temizlik yapar
