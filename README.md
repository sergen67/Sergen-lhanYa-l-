Git nedir<br>
2005 yılında ilk sürümü yayınlanan git,2009 yılına kadar linux ile iç içe olan dağıtık versiyon kontrol sistemiydi.2009 yılında GitHubın açık kaynak projeler için ücretsiz bir şekilde hizmet vermesi aynı yıllarda Bitbucket ve GitLabın benzer git servisleri sağlamaya başlaması geniş bir kitleye ulaşmasını sağladı.␣␣ <br>
dağıtık bir sürüm kontrol sistemidir.␣␣ <br>
herhangi bir klosör komutlarla yeni bir git dosya deposu haline gelebilir.␣␣ <br>
depolarda .git uzantısına sahip alt klasörler vardır.bu uzantıya sahip dosyalar güncel sürümleri ve eski sürümleri içerir.␣␣ <br>
kendi projenizi versiyon kontrolü altına almak istediğiniz de git init komutu ile bunu sağlayabiliriz␣␣ <br>
Windowsta git bash uygulaması ile yapılır.komutları aşağıda␣␣ <br>
$ cd proje/klasörünüzün/yolu/␣␣ <br>
$ git init␣␣ <br>
Repistory = projenin uzak bir sunucuda depolanması .kısaltılmış hali repo dur␣␣ <br>
Branch = Ana branch ve yan branch olarak ikye ayrılır.Bu yapı sayesinde ana yapıyı bozmadan yan branchlarla proje geliştirilebilir␣␣ <br>
Master= Reponun Ana alanı .␣␣ <br>
Commit = yapılan değişiklikleri saklayıp kaydedilmesine yarar.␣␣ <br>
Chechout = commitler üzerinden geçiş yapmamızı sağlar.␣␣ <br>
Fork = Reponun bir araya getirilmesidir.kopya üzerinde değişiklik yapıldıktan sonra ana depoya gönderilmesidir.␣␣ <br>
git init = bu komut ile proje dizininde git dizini oluşturulur.burada prijenin repo adresi,veriler vb. şeyler bullunur.␣␣ <br>
git add = eklemek istediğimiz dosyalar o dizine eklenmesini sağlar.␣␣ <br>
git rm = bir dosyayı dizinimizden kaldırmak için kullanılır.␣␣ <br>
git commit = yaptığımızdeğişiklikten sonra bu komut ile değişikliliği kaydederiz␣␣ <br>
git push = commitledğimiz dosyayı uzak sunucudaki repoya gönderir.␣␣ <br>
git pull = uzak sunucudaki dosyalarda bir değişiklik oluştuysa kendi local proje dosyaları ile birleştirir.␣␣ <br>
git merge = iki farklı branchı birleştirmeye yarar.␣␣ <br>
git clone = mevcut bir git reposunun bir kopyasını almak istediğimizde bu komutu kullanırız.␣␣ 


CI/CD NEDİR?␣␣ <br>
Sürekli entegrasyon ve Sürekli Dağıtım␣␣ <br>
CI(Sürekli Entegrasyon) = paylaşılan bir depoda kod değişikliklerini otomaik oluşturur,tes eder ve entegre eder.␣␣ <br>
CD(sürekli teslimat) = kod değişikliklerinde onay için otomatik olarak üretime hazır ortamlara iletir.␣␣ <br>
sürekli dağıtım (CD) = kod değişikliklerini doğrudan müşterilere otomatik olarak dağıtır.␣␣ <br>
Bunlar bir araya geldiğinde,Geliştirici ekiplerin manuel görevlerini azaltan otomatik bir sistem olan CI/CD hattı oluşur.␣␣ <br>
Sistemin tekrar eden sürümleri destekleyecek şekilde tasarlanmalı.␣␣ <br>
CI/CD kullanım␣␣ <br>
CI : Build + Test␣␣ <br>
dotnet restore paketleri çeker␣␣ <br>
dotnet build : projeyi derler␣␣ <br>
dotnet test : Unit testleri çalıştırır␣␣ <br>
CD: Publish + Deploy␣␣ <br>
dotnet publish : deploy edilecek klasörü hazırlar(Çalıştırabilir hale getirilir.)␣␣ <br>
Azure Web app'a atılır␣␣ <br>
Docker image oluşturulur␣␣ <br>
IIS'e deploy edilir␣␣ 





Azure DevOps␣␣ <br>
yazılım geliştiren ekipler için tümleşik araçlar sağlayan bulut tabanl bir platformdur␣␣ <br>
Temel Azure hizmetleri␣␣ <br>
-Azure Boards␣␣ <br>
-Azure Pipeline␣␣ <br>
-Azure Repos␣␣ <br>
-Azure Test plans␣␣ <br>
-Azure artifacts␣␣ <br>
Azure Boards␣␣ <br>
ekip arasında planlama ,izleme yapmak için kullanılır.birikmiş işler,özel raporlar için panolar oluşturulabilir.Bu panolar özlleştirilebilir ve izleme araçlarıyla anlamlı bilgiler edinebilirsin.␣␣ <br>
Azure Repos␣␣ <br>
kullanıcıların kod tabanlarını yönetmelerini sağlayan kod depolarıdır.Git sürüm kontrol sistemlerinide destekleyen bulut tabanlı depolardır.␣␣ <br>
Azure Pipeline␣␣ <br>
otomatik oluşturma,test etme ve dağıtım işlemlerini kolaylaştıran CI/CD aracıdır.␣␣ <br>
Azure Testplans␣␣ <br>
kullanıcıların test gereksinimlerini yönetebilmek için bulut tabanlı test platformunu entegre edebilemey olanak sağlar.␣␣ <br>
Azure Artifactss␣␣ <br>
paketleri oluşturmak, depolamak ve paylaşmak için kullanılan yapıt kitaplığı hizmetidirkullanıcıların tüm özelliklere sahip paket yönetimi işlevlerini CI/CD kanallarına entegre etmelerini sağlar.␣␣ 









SDLC nedir?␣␣ <br>
Bir yazılım geliştirme sürecindeki tüm faaliyetleri açıklayan kavram bütünüdür.Yüksek kalite ,etkili ve verimli yazılım geliştirmek ve zamanı minimum düzeyde tutmak için bir çerçevedir.Bu çerçeve belli aşamalrdan oluşurve her bir aşama bir sonraki aşamaya ürün bırakır.␣␣ <br>
AŞAMALAR:␣␣ <br>
1.ANALİZ␣␣ <br>
Yazılım geliştirme sürecinin ilk aşaması analizdir.Bu aşamada kullanıcı ihtiyaçları belirlenir ve bunlar nasıl karşılanır düşünülür.␣␣ <br>
2.PLANLAMA␣␣ <br>
analiz bittikten sonraplanlama kısmına geçilir.Bu aşamada projenin nasıl ilerleyeceğine dair plan yapılır.Planlama sürecinde hangi programlama dili kullanılıcağı,hangi araçların kullanılacağı ve ne kadar zaman süreceği planlanmaktadır.␣␣ <br>
3.TASARIM␣␣ <br>
planlama kısmı bittikten sonra tasarım kısmına geçilir.Bu aşamada arayüzler tasarlanır veya işlevler belirlenir.␣␣ <br>
4.GELİŞTİRME␣␣ <br>
Bu aşamada yazılım kodu yazılır.Geliştirme Sürecinde yazılımın kullanıcı ihtiyaçlarına yönelik olduğuna dairemin olunmalıdır.␣␣ <br>
5.TEST ETME␣␣ <br>
Bu aşamada ,yazılımın doğru çalışıp çalışmadığı kontrol edilir.hata olup olmadığı ,güvenliği,performansı gibi faktörler dikkate alınır.␣␣ <br>
AGİLE metodolojisi␣␣ <br>
Yazılım geliştirme projelerinde katı ve sabit planlar yerine , gereksinimlere göre değişen ortama hızlı uyum sağlamayı hedefleyen br metodolojidir.Proje küçük parçalara bölünerek her parça üzerinde ayrı ayrı çalışılır.takım çalışmasına teşvik eder ve ekip üyeleri arasında sürekli bir iletişim olur␣␣ <br>
SCRUM nedir?␣␣ <br>
Agile metodolojisinin parçası olan bir çerçevedir.bu çerçeve belirli roller ve yapılar etrafında organize edilir.kısa dögüler halinde çalışılır ve bu döngülere sprint adı verilir.her sprint sonunda hedeflenen ürün veya iş ortaya çıkar.␣␣ <br>
Scrum takımında Roller␣␣ <br>
1.Scrum Master : takımın kurallara uygun çalışmasını sağlar ve engelleri kaldırır.işbirliğini teşvik eder.Motivasyonu yüksek tutarak projenin hedeflerine ulaşmasını sağlar.␣␣ <br>
2.Product Owner:müşteri gereksinimini belirler.Müşteriden gelen feedbackleri toplar ve buna göre öncelikleri belirler.␣␣ <br>
3.Geliştirme Takımı :yazılım geliştiren ve teslim eden ekip üyelerinde oluşur.belirlenen hedeflere ulaşmak için birlikte çalışır ve her sprint sonunda işlevsel bir yazılım parçasını tamamlar.␣␣ 




GitHub Actions nedir?␣␣ <br>
yazılım geliştirme sürecinde otomatik iş akışları tanımlamak için kullanılan ,Github tarafından sağlanan bir CI/CD sistemidir.␣␣ <br>
Pipeline(İŞ akışı nedir?)␣␣ <br>
yazılım geliştirme sürecinde birbirini takip eden otomatik adımlar dizisidir.Github Actions da␣␣ <br>
pipline ,bir veya birden fazla görev ve bu görevlerin içinde yer alan steps(adımlar) biçiminde yapılandırılır.␣␣ <br>
3. Yapılandırma Dosyası␣␣ <br>
GitHub Actions iş akışları, projenin kök dizininde yer alan .github/workflows/ klasörü altında bir YAML dosyası olarak tanımlanır. Bu dosyada, iş akışının hangi olayla tetikleneceği, hangi sistemde çalışacağı ve hangi adımların gerçekleştirileceği belirtilir.␣␣ <br>
Örnek: Basit Bir "Hello World" Workflow␣␣ <br>
Bu örnek yapı, her push işlemi gerçekleştiğinde tetiklenir ve basit bir mesajı terminale yazdırır. Örnekte bir adet job ve onun içinde bir adet step yer almaktadır.␣␣ 




.Net Nedir?␣␣ <br>
.NET'in çeşitli uygulamaları, .NET kodunun Linux, macOS, Windows, iOS, Android ve diğer işletim sistemlerinde çalıştırılmasına izin verir.␣␣ <br>
.NET Tarihçesi␣␣ <br>
2000-2007␣␣ <br>
ilk beta sürümü 2000 yılının sonunda yayınlandı ve 13 Şubat 2002 de ilk sürüm olan .NET 1.0 yayınlandı.temel özelliği web uygulamalarının nesne yönelimli geliştirilmesini destekliyordu.␣␣ <br>
NET 1.1 (Nisan 2003): Bir dizi geliştirme (örneğin ASP.NET için güvenlik geliştirmeleri), İnternet Protokolü Sürüm 6 desteği ve ODBC içeriyordu.␣␣ <br>
.NET 2.0 (Kasım 2005): Genel koleksiyonlar, yineleyiciler, ASP.NET için yeni özellikler, geçersiz türler vb. içeriyordu.␣␣ <br>
.NET 3.0 (Kasım 2006): öne çıkanlar WPF (Windows Presentation Foundation), WCF (Windows Communication Foundation), WWF (Windows Workflow Foundation).␣␣ <br>
2007␣␣ <br>
kaynak kodu kullanıma sunuldu.Bu sürüme .NET3.5 adı verildi.bu sürümün temel özellikleri şunlardı:␣␣ <br>
AJAX desteği,␣␣ <br>
Dinamik veriler,␣␣ <br>
LINQ ␣␣ <br>
ASP.Net MVC␣␣ <br>
Microsoft, 2014 yılına kadar çerçevenin birkaç versiyonunu daha yayınladı:␣␣ <br>
.NET 4.0 (Nisan 2010): Yönetilen Genişletilebilirlik Çerçevesi, DLR, görev paralel kütüphanesi, Razor görünüm motoru.␣␣ <br>
.NET 4.5 (Ağustos 2012): Async desteği, daha iyi ASP.NET desteği, Zip sıkıştırma desteği, geliştirilmiş CLR 4.0␣␣ <br>
.NET 4.5.1 (Ekim 2013): daha iyi performans ve hata ayıklama, Windows Mağazası uygulama geliştirme için gelişmiş destek.␣␣ <br>
2014 .NET Core'un başlangıcı␣␣ <br>
Bu zamana kadar .NET ' in en büyük kusuru windows dışındaki platformlarda çalışamamsıdır.Bu sorunu çözmek için Microsoft 2014 yılında .NET Core duyurdu.␣␣ <br>
.NET ile neler yapılabilir?␣␣ <br>
.NET ile kullanarak şu uygulamalar geliştirilebilir:␣␣ <br>
Windows Uygulamaları,␣␣ <br>
Windows Phone Uygulamaları,␣␣ <br>
Web Uygulamaları (ASP.Net),␣␣ <br>
Oyunlar␣␣ <br>
Mobil Uygulamalar␣␣ <br>
Windows Azure ile cloud uygulamaları,␣␣ <br>
MS Office için eklentiler,␣␣ <br>
Veri tabanı uygulamaları ␣␣ <br>
.NET'in avantajları Nelerdir?␣␣ <br>
Geliştirme Kolaylığı␣␣ <br>
Zaman Tasarufu␣␣ <br>
Yüksek performanslı uygulamalar oluşturma␣␣ <br>
Güvenilirlik␣␣ <br>
Zengin Kaynak ve kitaplıklar␣␣ <br>
Topluluk desteği␣␣ 


<img width="554" height="479" alt="image" src="https://github.com/user-attachments/assets/c2a31f66-db2a-49e5-b500-2b2773b17c3a" />





Senkron ve Asenkron Programlama<br>
Senkron Programlama<br>
-İşlemler Sırasıyla yapılır.Bir işlem bitmeden diğer işleme geçilemez.Doğrusal ve anlaşılması kolaydır.Ağır görevlerde işleri yavaşlatabilir ve gecikmelere neden olabilir.<br>
Asenkron Programlama<br>
-Asenkron programlama , birden fazla belgenin aynı anda işlenmesi gibi zaman alan işlemleri gerçekleştirmek içindir.Tarayıcılar buna bir örnek olabilir.<br>
Temel anahtar kavramlar<br>
1.async<br>
bir metodun asenkron olduğunu gösterir. Geri dönüş tipi Task ' dır<br>

public async Task<string> VeriGetirAsync()<br>
{<br>
await Task.Delay(1000); // simülasyon<br>
return "Veri hazır";<br>
}<br>
2.await<br>
asenkron işlemi başlatmaya yarar.sonucu beklerken thread kilitlenemez<br>
3.Task<br>
Sonuç dndüremeyen işlemler için kullanılır.<br>
4. ConfigureAwait<br>
UI thread veya synchronization context gerekmeyen yerlerde performans ve deadlock riski için önemlidir<br>
C#’ta => (Arrow Function) İfadesi<br>
Bu operatör , lambda ifadelerinde ve kısa method tanımlamalarında geçer.<br>
1. Lambda ifadesi<br>
Func<int, int> karesi = x => x * x;<br>
Console.WriteLine(karesi(5)); // 25<br>
2. Kısa method<br>
public int Topla(int a, int b) => a + b;<br>
3. Property<br>
public string Ad => "baba"; // readonly, expression-style property<br>



dotnet --info çıktısı örneği ve yorumlama<br>

.NET SDK (reflecting any global.json):  Version:   8.0.100  // Şu anda kullanılan SDK sürümünü belirler<br>
Commit:    3d885d3f90  <br>
Runtime Environment: <br>
OS Name:     Windows // hangi işletim sistemi üzerinde çalıştığımızı gösterir <br>
OS Version:  10.0.22621 //İşletim sisteminin sürümünü gösterir  <br>
OS Platform: Windows  RID:         win10-x64 //Proje hangi sistem için build edileceğini gösterir  <br>
Base Path:   C:\Program Files\dotnet\sdk\8.0.100\ //SDK nın kurulu olduğu dosya yolunu gösteri <br>
Host:  <br>
Version:      8.0.0  <br>
Architecture: x64   <br>
Commit:       5678abcd12  <br>
.NET SDKs installed:// Makinede kurulu Tüm SDK sürümlerini gösterir   6.0.416 [C:\Program Files\dotnet\sdk]   7.0.306 [C:\Program Files\dotnet\sdk]   8.0.100 [C:\Program Files\dotnet\sdk] <br>
.NET runtimes installed://çalıştırmak için gerekli runtime'ları listeler   <br>
Microsoft.AspNetCore.App 6.0.16 [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App] <br>
Microsoft.AspNetCore.App 7.0.9  [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]   <br>
Microsoft.AspNetCore.App 8.0.0  [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]  <br>
Microsoft.NETCore.App 6.0.16    [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]   <br>
Microsoft.NETCore.App 7.0.9     [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]  <br>
Microsoft.NETCore.App 8.0.0     [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]<br>
Other architectures found: alternatif kurulumları gösterir.   <br>
x86   [C:\Program Files (x86)\dotnet\] <br>
Environment variables: Sistemdeki çevre değişkenlerini gösterir.  <br>
DOTNET_ROOT = C:\Program Files\dotnet<br>


BackEnd nedir?<br>
Backend ,kullanıcının web sitesinde veya bir uygulamada kullanırken görmediği ama uygulamanın düzgün çalışmasını sağlayan kaynak kodlar ve veritabanından oluşan kısımdır.<br>
Veritabanının ve uygulamanın birbiri ile iletişime geçmesini sağlayan ,sorunsuz çalışmasını sağlayan kodlardan oluşur.<br>
FrontEnd ve BackEnd farkı<br>
bu ikisi arasındaki temel farklar ilgilendikleri alan ve teknolojilerdir.Frontedn Kullanıcın etkileşime girdiği kısımla ilgilenirken,backend daha ço uygulamanın işlemlerinin nasıl gerçekleşeceğiyle ilgili kısımdan sorumludur.<br>
<br>
Web Sunucusu nedir?<br>
internet ortamında web sitesinin yayınlanmasından sorumlu olan sunucudur.Hosting işlemini internet protokolü üzerinden yapar.Hosting,Web sitelerinin yayınlanmak için gerekli alanı kiralamasıdır.<br>



API nedir?<br>
İki yazılım projesinin birbirleriyle iletişim kurmasını sağlayan bir nevi anahtardır.<br>
API türleri<br>
-Özel API'ler<br>
Yalnızca kullanılacak olan işletmenin içindeki sistem ve verileri bağlamak için kullanılır.<br>
-Genel API'ler<br>
halka açık,herkesin kullanabileceği API türüdür.<br>
-Çözüm Ortağı API'ler<br>
işletmeler arası yardım sağlamak amaçlı kullanılar API'lerdir.<br>
-Birleşik API'LER<br>
karmaşık sistemler için iki veya daha fazla AOI'yi bir araya getirir.<br>

HTTP nedir?<br>
HTTP ,WWW'in temelini oluşturur.Köprü metni bağlantıları kullanarak web sayfalarını kullanır.Cihazlar arasında bilgi aktarım için kullanılır.İstemcinin sunucuya istekte bulunmasını ve sunucunun bir geri bildirim vermesini sağlar.<br>
HTTP metodları<br>
-GET<br>
Sunucudan veri istemek için kullanılır<br>
GET /search?q=security+engineer HTTP/1.1<br>
Host: google.com<br>
bu ısımda veri URL'nin içine gömülüyor.sunucudan security engineer arama sonuçları isteniyor<br>
-POST<br>
Sunucuya veri göndermek için kullanılır<br>
POST /login HTTP/1.1<br>
Host: example.com<br>
Content-Type: application/json<br>

{<br>
"username": "baba",<br>
"password": "hunter2"<br>
}<br>
Veri burada get'deki gibi URL'de değil body kısmında taşınır.<br>
-PUT<br>
sunucuya bir kaynağı yerleştirmek için kullanılır.<br>
PUT /api/users/123 HTTP/1.1<br>
Content-Type: application/json<br>

{<br>
"id": 123,<br>
"username": "baba",<br>
"email": "baba@cybermail.io"<br>
}<br>
-DELETE<br>
Sunucudaki bir veriyi silmek için kullanılır.<br>
DELETE /api/users/123 HTTP/1.1<br>
bu kodda da id'si 123 olan kullanıcıyı siliyor.<br>
JSON nedir?<br>
JSON bir kod bloğu değildir.Depoları saklamak ve aktarmak için kullanılır.Farklı programlama dilleri arasına rahatlıkla veri değişimi sağlar.Genellikle web uygulamaları ve sunucular arasında veri göndermek için kullanılır.<br>
JSON veri tipleri<br>
-Nesneler<br>
-Diziler<br>
-Dizeler<br>
-Mantıksal değer<br>
-Null<br>
-Sayı<br>
örnek<br>
<br>
{<br>
"name": "Sergen İlhan Yağlı",<br>
"age": 21,<br>
"city": "Bursa",<br>
"phone": "5511711763",<br>
"email": sergenilhany67@gmail.com"<br>
}<br>


REST vs SOAP vs GraphQL<br>
REST http +JSON/XMl kullanırken SOAP XML+WS kullanır GraphQL ise HTTP+JSON kullanır<br>
veri formatları Rest'te JSON veya XML SOAP ta ise sadece XML GraphQL de ise sadece JSON kullanılır.<br>
REST 'te güvenlik HTTPS ,OAuth ,JWT ile sağlanır,SOAP ta ise WS-Security ile,GraphQL'de ise HTTPS ,OAuth ,JWT ile sağlanır.<br>


Dependency Injection Kullanımına Örnek<br>
public interface ILogger<br>
{<br>
void Log(string message);<br>
}<br>
bir interface oluşturuyoruz<br>
public class ConsoleLogger : ILogger<br>
{<br>
public void Log(string message)<br>
{<br>
Console.WriteLine("Log: " + message);<br>
}<br>
}<br>
önceki interface'e bağlı bir sınıf yazıyoruz<br>
public class Game<br>
{<br>
private readonly ILogger _logger;<br>
<br>
// DI burada: logger dışarıdan veriliyor<br>
public Game(ILogger logger)<br>
{<br>
_logger = logger;<br>
}<br>

public void Start()<br>
{<br>
_logger.Log("Oyun başladı!");<br>
}<br>
}<br>


Performans için önerilen en az 3 teknik ve açıklamaları<br>
1.AsNoTracking()<br>
EF Core ,default ayar olarak her veriyi takip eder.Ama sadece veriyi okuma işlemi yapacaksan bu çok gereksiz bir yük olur.<br>
bu tekniği kullanırsan sorgulama neredeyse %50 hızlanır ,bellek tüketimi azalır.<br>
2.Caching<br>
Aynı veriyi sürekli sorguluyorsak bu zaman ve kaynak kaybıdır.Caching ile bu durumun önüne geçiyoruz.Bu sayede DB sor<br>gu sayısı azalır.<br>
3.DTO+Select<br>
EF'de bir entity'yi doğrudan çağırırsan tüm alanları çekmiş olursun buda bellekteki yükü arttırır.Bu teknik sayesinde sadece gerekli alanlar çekilir.Ağ trafiğide düşer.<br>


OWASP 10 listesi ve her biri için 1–2 cümlelik açıklamalar<br>
1.Brokjen Access Control<br>
Kullanıcı,yetkisi olmayan alanlara erişebilme durumudur.<br>
2.Cryptographic Failures<br>
Veriler doğru şifrelenemiyor veya hiç şifrelenemme durumudur.<br>
3.Injection<br>
Kullanıcıgirişi doğrudan sorguya eklendiği için sxaldırgan komut enjekte edebilir.<br>
4.Insecure Design<br>
Uygulamanın en baştan beri güvenliğe uygun dizayn edilmemesidir.<br>
5.Security Misconfiguration<br>
Güvenlik ayarlarının eksik,yanlış veya varsayılan bırakılmasıdır.<br>
6.Vulnurable and Outdated Components<br>
Kullanılan kütüphane veya yazılımların eski veya bilinen açıkları içermesidir.<br>
7.Identification and authentication Faailures<br>
Kimlik doğrulama sistemi zayıf olduğunda saldırganların kolayca hesaplara erişebilmesidir<br>
8.Software and Data ıntegrity Failures<br>
uygulama güncellemeleri,kod veya veriler doğrulama yapılmadan çalıştırılması.<br>
9.Security logging and Monitoring Failures<br>
Loglama eksik veya olmadığından saldırı girişimleri tespit edilememesidir.<br>
10.Server-Side Request Forgery<br>
Saldırganın sunucunun farklı adreslere istek göndermesini sağlayabiliyor.<br>

Her SOLID prensibi için kısa örnek<br>
Single responsibility Principle(SRP)<br>
bir sınıfın sadece bir sorumluluğa sahip olması<br>
örn<br>
class ReportGenerator { public void Generate() { } }<br>
class ReportSaver { public void SaveToFile() { } }<br>
Open/Closed Principle(OCP)<br>
sınıfların geliştirmeye açık değişime kapalı olması<br>
örn<br>
interface IDiscount { double GetRate(); }<br>

class RegularDiscount : IDiscount { public double GetRate() => 1.0; }<br>
class PremiumDiscount : IDiscount { public double GetRate() => 0.8; }<br>

class DiscountCalculator<br>
{<br>
public double Calculate(IDiscount discount) => discount.GetRate();<br>
}<br>
Liskov Substitution Principle<br>
türeyen sınıf,ana sınıfın yerine sorunsuz geçebiliyor olmalı<br>
örn<br>
interface IBird { }<br>
interface IFlyingBird : IBird { void Fly(); }<br>

class Sparrow : IFlyingBird { public void Fly() { } }<br>
class Ostrich : IBird { }<br>
Interface Segregation Principle<br>
arayüzler küçük ve öz olmalı,kullanılmayan metotlar içermemeli<br>
örn<br>
interface IWorkable { void Work(); }<br>
interface IEatable { void Eat(); }<br>

class Robot : IWorkable { public void Work() { } }<br>
Dependency Inversion Principle<br>
Üst Sınıflar ,soyutlamalara bağlı kalmalı somut sınıflara değil<br>
örn<br>
interface IMessageService { void Send(); }<br>

class EmailService : IMessageService { public void Send() { } }<br>

class Notification<br>
{<br>
private IMessageService _service;<br>
public Notification(IMessageService service) { _service = service; }<br>
public void Alert() => _service.Send();<br>
}<br>


En az 2 design pattern açıklaması<br>
1.Singleton pattern<br>
Uygulama boyunca instance olmasını istediğin tek bir sınıf için kullanılır.<br>
Amaç:Belleğimde sadece 1 sınıf olsun ve tüm sistem ortak kullansın<br>
2.Strategy pattern<br>
Değişken algoritmaları runtime içinde seçilebilir hale getirir.Örn:İndirim hesaplamaları<br>
Amaç:farklı algoritmalar birbirinin yerini sorunsuz bir şekilde alır.<br>

Clean Code uygulama örnekleri<br>
Anlamlı isimlendirme<br>
Örn<br>
İnt d;<br>
burada tam olarak neyi tanımladığımız belli olmayabilir ama<br>
int arabaModel;<br>
gibi daha açık tanımlama yaparsak değişkenlere daha temiz olur.<br>
Fonksiyonlar kısa ve tek iş yapmalı<br>
void HandleUser()<br>
{<br>
Validate();<br>
Save();<br>
SendEmail();<br>
}<br>
burada fonksiyonlara genel bir tanımlama yapılmış<br>
void HandleUser()<br>
{<br>
ValidateUser();<br>
SaveUser();<br>
SendWelcomeEmail();<br>
}<br>
böyle daha iyi.<br>
Gereksiz yorum satırı ekleme<br>
// kullanıcıya e-posta gönderir<br>
SendEmail();<br>
bunu açıklamak yerine fonksiyon isminden ne olduğunu anlayalım<br>
SendWelcomeEmail();<br>

			

<img width="513" height="365" alt="image" src="https://github.com/user-attachments/assets/7021e8cd-f2cd-4189-aa47-31db9c056503" />

				


Log seviyelerinin açıklamaları<br>
-Debug<br>
geliştime sırasında kullanılan adımlarını tek tek göstermeye yarayan bir log<br>
-ınformation<br>
uygulamanın normal işleyişini bildirir.Önemli olayları loglar.<br>
-Warning<br>
Şüpheli olan durumları bildirir bu durularda sistem çalışmaya devam eder ama ileride sıkıntı çıkarabilir.<br>
-Error<br>
Hata logudur.Sistemde bir şeylerin yanlış veya eksik olduğunu gösterir.<br>


Örnek hata yönetim kodu  açıklaması<br>

public User GetUserById(int id)<br>
{<br>
try<br>
{<br>
// DB'den kullanıcıyı çek<br>
var user = dbContext.Users.First(u => u.Id == id);<br>

// Kullanıcı bulunursa döndür<br>
return user;<br>
}<br>
catch (InvalidOperationException)<br>
{<br>
// Kullanıcı yoksa (First() patlar)<br>
Console.WriteLine($"Hata: ID {id} ile kullanıcı bulunamadı.");<br>
return null;<br>
}<br>
catch (Exception ex)<br>
{<br>
// Beklenmeyen her şeyi burası yakalar<br>
Console.WriteLine("Beklenmeyen hata: " + ex.Message);<br>
return null;<br>
}<br>
finally<br>
{<br>
// Her durumda çalışır (başarılı ya da hata)<br>
Console.WriteLine("GetUserById çalışması tamamlandı.");<br>
}<br>
}<br>
try: Riskli kod kodlar buraya yazılır.<br>
catch : hata oluşursa buraya gelir.birden fazla olabilir bü yüzden tipi önemlidir.<br>
catch(InvalıdOperationException) : First() kullanıcı bulamazsa bu hatayı verir<br>
catch (exception ex) : genelhata yakalama.Özel türler önce yazılır,en sona gelir.<br>
finally: hata olsada olmasada çalışır.temizlik yapar<br>
