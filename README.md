![unity](Images\WindowsCMDForUnity.png "Unity Windows")

# Unity Geliştiricileri İçin Kullanışlı Windows Komutları

## Amaç
Bu paylaşımın amacı unity geliştiricileri için kullanışlı olabileceğini düşündüğüm Windows komutları paylaşmaktır.

## `cd` Komutu
`cd` komutu ile klasörler arasında geçiş yapabiliyoruz. Bu komutun işlevleri şu şekildedir:
* `cd` komutu `cd..` ile bir üst klasörü geçiş yapabiliyoruz. 
* `cd.` komutu ile bulunduğumuz klasörü gidebiliyoruz. 
* `cd /` komutu ile C: klasörüne gidebiliyoruz. 

![cd_komutu](https://user-images.githubusercontent.com/69583116/102006550-9860 "cd Komutu")

## `mkdir` Komutu
`mkdir` komutu ile klasör oluşturabiliyoruz. Bu komutun işlevleri şu şekildedir:

```Shell
mkdir <klasör_adı>
```

![mkdir_komutu](https://user-images.githubusercontent.com/69583116/102006551-9860 "mkdir Komutu")

## `dir` Komutu
`dir` komutu ile klasörlerde bulunan dosyaları ve klasörleri görebiliyoruz. Bu komutun işlevleri şu şekildedir:

* `dir` komutu: Bu, temel `dir` komutudur. Mevcut dizindeki dosyaları ve klasörleri listeler. Gizli dosyaları ve sistem dosyalarını varsayılan olarak göstermez.

* `dir /a` komutu: "/a" parametresi "all" (tümü) anlamına gelir. Bu komut, gizli dosyalar ve sistem dosyaları da dahil olmak üzere mevcut dizindeki tüm dosyaları ve klasörleri gösterir.

* `dir /a-d` komutu: Bu komut, sadece dosyaları gösterir, klasörleri göstermez. "/a-d" parametresindeki "-d" kısmı "directories" (klasörler) anlamına gelir ve bunları hariç tutar.

* `dir /a-h` komutu: Bu komut, gizli olmayan tüm dosyaları ve klasörleri gösterir. "/a-h" parametresindeki "-h" kısmı "hidden" (gizli) anlamına gelir ve gizli dosyaları hariç tutar.

Her bir komutun çıktısı farklı olacaktır:
- Temel `dir` komutu normal dosyaları ve klasörleri gösterir.
- `dir /a` hem normal hem de gizli ve sistem dosyalarını gösterir.
- `dir /a-d` sadece dosyaları gösterir, klasörleri göstermez.
- `dir /a-h` gizli olmayan tüm öğeleri (dosyalar ve klasörler) gösterir.

Bu komutlar, özellikle Unity projeleri üzerinde çalışırken, proje yapısını incelemek, gizli dosyaları kontrol etmek veya sadece belirli türdeki öğeleri listelemek için kullanışlı olabilir.
* `dir /a-d` komutu ile klasörlerde bulunan dosyaları ve klasörleri görebiliyoruz. 
* `dir /a-h` komutu ile klasörlerde bulunan dosyaları ve klasörleri görebiliyoruz. 

![dir_komutu](https://user-images.githubusercontent.com/69583116/102006552-9860 "dir Komutu")

## `copy` Komutu
`copy` komutu ile dosyaları kopyalamak için kullanılır. Bu komutun kullanımı şu şekildedir:

```Shell
copy <kaynak_dosya> <hedef_dosya>
```

![copy_komutu](https://user-images.githubusercontent.com/69583116/102006553-9860 "copy Komutu")

## `move` Komutu
`move` komutu ile dosyaları taşımak için kullanılır. Bu komutun kullanımı şu şekildedir:

```Shell
move <kaynak_dosya> <hedef_dosya>
```

![move_komutu](https://user-images.githubusercontent.com/69583116/102006554-9 "move Komutu")

## `ipconfig` Komutu
`ipconfig` komutu ile tüm geçerli TCP/IP ağ yapılandırma değerlerini görüntüler ve Dinamik Ana Bilgisayar Yapılandırma Protokolü (DHCP) ve Etki Alanı Adı Sistemi (DNS) ayarlarını yeniler. Parametreler olmadan kullanıldığında, ipconfig tüm bağdaştırıcılar için İnternet Protokolü sürüm 4 (IPv4) ve IPv6 adreslerini, alt ağ maskesini ve varsayılan ağ geçidini görüntüler.

![ipconfig_komutu](https://user-images.githubusercontent.com/69583116/102006554-9860 "ipconfig Komutu")

## `del` Komutu
`del` komutu ile belitririlen dosya silinir. Bu komutun kullanımı şu şekildedir:

```Shell
del <kaynak_yol>
```

![del_komutu](https://user-images.githubusercontent.com/69583116/102006553-9860 "del Komutu")

## `tasklist` Komutu
`tasklist` komutu ile bilgisayarda çalışan sistemleri listeler.

![tasklist_komutu](https://user-images.githubusercontent.com/69583116/102006554-986 "tasklist Komutu")

## `taskkill` Komutu
`taskkill` komutu, Windows'ta çalışan işlemleri (processes) sonlandırmak için kullanılır. Bu komut, özellikle yanıt vermeyen programları kapatmak veya belirli işlemleri sonlandırmak için kullanışlıdır. İşte `taskkill` komutunun çeşitli kullanım şekilleri:

* `taskkill /im <process_name>`: Bu komut, belirtilen isme sahip işlemi nazikçe kapatmaya çalışır. İşlem normal şekilde kapatılır.
  Örnek: `taskkill /im notepad.exe`

* `taskkill /f /im <process_name>`: "/f" parametresi "force" (zorla) anlamına gelir. Bu komut, belirtilen işlemi zorla kapatır. İşlem anında sonlandırılır.
  Örnek: `taskkill /f /im chrome.exe`

* `taskkill /f /im <process_name> /t`: "/t" parametresi "tree" (ağaç) anlamına gelir. Bu komut, belirtilen işlemi ve onun başlattığı tüm alt işlemleri zorla kapatır.
  Örnek: `taskkill /f /im explorer.exe /t`

* `taskkill /f /im <process_name> /pid <process_id>`: Bu komut, belirli bir işlem kimliğine (PID) sahip belirli bir işlemi zorla kapatır.
  Örnek: `taskkill /f /im chrome.exe /pid 1234`

* `taskkill /f /im <process_name> /pid <process_id> /t`: Bu komut, belirli bir PID'ye sahip işlemi ve onun tüm alt işlemlerini zorla kapatır.
  Örnek: `taskkill /f /im chrome.exe /pid 1234 /t`

Bu komutlar, özellikle Unity geliştirme sürecinde yanıt vermeyen Unity uygulamalarını veya editörünü kapatmak, performans sorunlarına neden olan arka plan işlemlerini sonlandırmak veya test amaçlı olarak belirli işlemleri kontrollü bir şekilde kapatmak için kullanışlı olabilir.

Not: İşlemleri zorla kapatmak veri kaybına neden olabilir, bu nedenle dikkatli kullanılmalıdır.

![taskkill_komutu](https://user-images.githubusercontent.com/69583116/102006554-9860 "taskkill Komutu")

## `ping` Komutu
`ping` komutu ile belirli bir sunucuya bağlanma ve yanıt alma durumlarını kontrol etmek için kullanılır. Bu komutun kullanımı şu şekildedir:
* `ping <sunucu_adresi>`: Bu komut, belirtilen sunucuya bağlanma ve yanıt alma durumlarını kontrol eder
* `ping <sunucu_adresi> -t`: Bu komut, belirtilen sunucuya bağlanma ve yanıt alma durumlarını kontrol eder ve her saniye bir kez yanıt alma durumunu kontrol eder.
* `ping <sunucu_adresi> -n <saniye_sayisi>`: Bu komut, belirtilen sunucuya bağlanma ve yanıt alma durumlarını kontrol eder ve belirtilen saniye sayısı kadar yanıt alma durumunu kontrol eder.

![ping_komutu](https://user-images.githubusercontent.com/69583116/102006555-9860 "ping Komutu")

## `systeminfo` Komutu
`systeminfo` komutu ile bilgisayarın bilgilerini görüntüler. Bu komutun kullanımı şu şekildedir:
* `systeminfo`: Bu komut, bilgisayarın işletim sistemi, işlemci, ana bilgisayar, kullanıcı, sürücü ve disk bilgisini, görüntüsü ve bağlantı bilgilerini görüntüler.
* `systeminfo /fo csv`: Bu komut, bilgisayarın işletim sistemi, işlemci, ana bilgisayar, kullanıcı, sürücü ve disk bilgisini, csv (comma-separated values) biçiminde görüntüler.
* `systeminfo /fo list`: Bu komut, bilgisayarın işletim sistemi, işlemci, ana bilgisayar, kullanıcı, sürücü ve disk bilgisini, listeleri (table) biçiminde görüntüler.

![systeminfo_komutu](https://user-images.githubusercontent.com/69583116/102006556- "systeminfo Komutu")

## `tree` Komutu
`tree` komutu, bir dizinin yapısını görsel olarak gösteren kullanışlı bir Windows komutudur. Bu komut, özellikle karmaşık proje yapılarına sahip Unity projelerinde dosya ve klasör hiyerarşisini anlamak için çok faydalı olabilir. İşte `tree` komutunun çeşitli kullanım şekilleri:

* `tree <dizin_yolu>`: Bu temel komut, belirtilen dizinin alt dizinlerini ve klasör yapısını gösterir. Dosyaları göstermez.
  Örnek: `tree C:\UnityProjects\MyGame`

* `tree <dizin_yolu> /f`: "/f" parametresi "files" (dosyalar) anlamına gelir. Bu komut, dizin yapısını gösterirken her klasördeki dosyaları da listeler.
  Örnek: `tree C:\UnityProjects\MyGame /f`

* `tree <dizin_yolu> /a`: "/a" parametresi "ASCII" anlamına gelir. Bu komut, dizin yapısını gösterirken ASCII karakterleri kullanır. Bu, özellikle çıktıyı bir metin dosyasına yönlendirirken veya bazı konsolların grafik karakterleri düzgün göstermediği durumlarda faydalıdır.
  Örnek: `tree C:\UnityProjects\MyGame /a`

* `tree <dizin_yolu> /a /f`: Bu komut, ASCII karakterleri kullanarak hem dizin yapısını hem de dosyaları gösterir.
  Örnek: `tree C:\UnityProjects\MyGame /a /f`

Unity geliştiricileri için `tree` komutunun kullanım örnekleri:

1. Proje yapısını incelemek:
   `tree C:\UnityProjects\MyGame\Assets`

2. Script dosyalarının organizasyonunu görmek:
   `tree C:\UnityProjects\MyGame\Assets\Scripts /f`

3. Prefab ve sahne dosyalarının yerleşimini kontrol etmek:
   `tree C:\UnityProjects\MyGame\Assets\Prefabs C:\UnityProjects\MyGame\Assets\Scenes /f`

4. Projenin genel yapısını bir metin dosyasına kaydetmek:
   `tree C:\UnityProjects\MyGame /a /f > project_structure.txt`

Bu komut, özellikle büyük Unity projelerinde dosya organizasyonunu anlamak, proje yapısını dokümante etmek veya farklı projeler arasında yapı karşılaştırması yapmak için çok kullanışlıdır.

Not: Çok büyük projelerde `/f` parametresini kullanırken dikkatli olun, çünkü çıktı oldukça uzun olabilir.

![tree_komutu](https://user-images.githubusercontent.com/69583116/102006557-9860 "tree Komutu")

## `driverquery` Komutu
`driverquery` komutu, Windows işletim sisteminde yüklü olan sürücülerin (drivers) listesini görüntülemek için kullanılır. Bu komut, özellikle Unity geliştiricileri için donanım uyumluluğu ve performans sorunlarını teşhis etmede yararlı olabilir. İşte `driverquery` komutunun çeşitli kullanım şekilleri:

* `driverquery`: Bu temel komut, sistemde yüklü olan tüm sürücülerin basit bir listesini gösterir.

* `driverquery /v`: "/v" parametresi "verbose" (ayrıntılı) anlamına gelir. Bu komut, sürücüler hakkında daha detaylı bilgi sağlar, örneğin sürücü sağlayıcısı, sürücü versiyonu ve sürücü türü gibi.

* `driverquery /fo csv`: "/fo csv" parametresi, çıktıyı CSV (Comma-Separated Values) formatında oluşturur. Bu, sürücü bilgilerini Excel gibi bir uygulamada analiz etmek isteyenler için kullanışlıdır.
  Örnek: `driverquery /fo csv > drivers.csv`

* `driverquery /si`: "/si" parametresi "signed" (imzalı) anlamına gelir. Bu komut, dijital olarak imzalanmış sürücüler hakkında bilgi verir, ki bu güvenlik açısından önemlidir.

Unity geliştiricileri için `driverquery` komutunun kullanım örnekleri:

1. Grafik sürücülerini kontrol etmek:
   `driverquery | findstr "display"`

2. Ses sürücülerini incelemek:
   `driverquery | findstr "audio"`

3. Tüm sürücüleri ayrıntılı bir şekilde bir CSV dosyasına kaydetmek:
   `driverquery /v /fo csv > unity_system_drivers.csv`

4. İmzalanmamış sürücüleri tespit etmek (potansiyel güvenlik riskleri):
   `driverquery /si | findstr "FALSE"`

Bu komut, Unity projelerinde performans sorunları yaşandığında, özellikle grafik veya ses ile ilgili problemlerde, sistemdeki sürücülerin durumunu kontrol etmek için kullanılabilir. Ayrıca, farklı test ortamları arasında sürücü uyumluluğunu karşılaştırmak için de faydalıdır.

Not: Sürücülerle ilgili herhangi bir değişiklik yapmadan önce, sistem yedeği almak ve dikkatli olmak önemlidir.

![driverquery_komutu](https://user-images.githubusercontent.com/69583116/102006558-9860 "driverquery Komutu")

## `getmac` Komutu
`getmac` komutu, Windows işletim sistemindeki MAC adresini (Media Access Control) görüntüler. Bu komut, özellikle Unity geliştiricileri mac adreslerini, dizinleri ve diğer bağlantıları kontrol etmek için kullanışlıdır. İşte `getmac` komutunun çeş itli kullanım şekilleri:

* `getmac`: Bu temel komut, sistemdeki herhangi bir MAC adresini görüntüler.
* `getmac /all`: "/all" parametresi, sistemdeki tüm MAC adreslerini görüntüler.
* `getmac /v`: "/v" parametresi, MAC adreslerini daha detaylı bir şekilde görüntüler.
* `getmac /fo csv`: "/fo csv" parametresi, MAC adreslerini CSV (Comma-Separated Values) formatında görüntüler.

![getmac_komutu](https://user-images.githubusercontent.com/69583116/102006559- "getmac Komutu")

## `powercfg` Komutu
`powercfg` komutu, Windows işletim sistemindeki performans ve güvenlik ayarlarını yönetmek için kullanılır. Bu komut, özellikle Unity geliştiricileri performans ve güvenlik ayarlarını değiştirmek için kullanışlıdır. İşte `powercfg` komutunun çeşitli kullanı şekilleri:

* `powercfg`: Bu temel komut, sistemdeki tüm performans ve güvenlik ayarlarını listeler.
* `powercfg /a`: "/a" parametresi, sistemdeki tüm performans ayarlarını listeler.
* `powercfg /q`: "/q" parametresi, sistemdeki tüm güvenlik ayarlarını listeler.
* `powercfg /h`: "/h" parametresi, sistemdeki tüm performans ve güvenlik ayarlarını yeniden başlatır.
* `powercfg /h /a`: "/h /a" parametresi, sistemdeki tüm performans ayarlarını yeniden başlatır.
* `powercfg /h /q`: "/h /q" parametresi, sistemdeki tüm güvenlik ayarlarını yeniden başlatır.

![powercfg_komutu](https://user-images.githubusercontent.com/69583116/102006560- "powercfg Komutu")

## `wmic` Komutu
`wmic` (Windows Management Instrumentation Command-line) komutu, Windows sistemlerinde sistem yönetimi ve bilgi toplama için güçlü bir araçtır. Unity geliştiricileri için, özellikle donanım bilgilerini toplamak, sistem durumunu kontrol etmek ve otomatik görevler oluşturmak için kullanışlıdır. İşte `wmic` komutunun Unity geliştiricileri için önemli kullanım örnekleri:

1. Sistem Bilgilerini Almak:
   * `wmic computersystem get model,name,manufacturer,systemtype`: Bilgisayarın modelini, adını, üreticisini ve sistem türünü gösterir.
   * `wmic os get caption,version,osarchitecture`: İşletim sistemi adını, sürümünü ve mimarisini gösterir.

2. Donanım Bilgilerini Kontrol Etmek:
   * `wmic cpu get name,numberofcores,maxclockspeed`: İşlemci adını, çekirdek sayısını ve maksimum hızını gösterir.
   * `wmic memorychip get capacity,speed`: RAM kapasitesini ve hızını gösterir.
   * `wmic diskdrive get model,size,status`: Sabit disk modelini, boyutunu ve durumunu gösterir.

3. Grafik Kartı Bilgilerini Almak:
   * `wmic path win32_VideoController get name,adapterram,driverversion`: Grafik kartı adını, RAM'ini ve sürücü sürümünü gösterir.

4. Çalışan Uygulamaları Listelemek:
   * `wmic process where "name like '%Unity%'" get name,processid,commandline`: Çalışan Unity ile ilgili süreçleri listeler.

5. Sistem Performansını İzlemek:
   * `wmic cpu get loadpercentage`: CPU kullanım yüzdesini gösterir.
   * `wmic memorychip get capacity`: Toplam RAM kapasitesini gösterir.

6. Unity Projesi için Otomatik Görevler:
   * `wmic process call create "C:\Program Files\Unity\Hub\Editor\2021.3.0f1\Editor\Unity.exe -projectPath C:\UnityProjects\MyGame -batchmode -quit -logFile C:\buildlog.txt -buildWindows64Player C:\Builds\MyGame.exe"`: Unity projesini komut satırından derler.

7. Sistem Günlüklerini İncelemek:
   * `wmic nteventlog get path,filename,writedate`: Sistem olay günlüklerini listeler.

Bu komutlar, Unity geliştiricilerinin sistem durumunu analiz etmelerine, performans sorunlarını teşhis etmelerine ve otomatik derleme süreçleri oluşturmalarına yardımcı olabilir. Ayrıca, farklı test ortamlarında tutarlı sistem bilgileri toplamak için de kullanışlıdır.

Not: Bazı `wmic` komutları yönetici ayrıcalıkları gerektirebilir. Ayrıca, Microsoft Windows 11'de `wmic` yerine daha modern `Get-WmiObject` PowerShell cmdlet'i kullanılması önerilmektedir.

![wmic_komutu](https://user-images.githubusercontent.com/69583116/102006561-9860 "wmic Komutu")

## `sc queryex type=service state=all` Komutu
`sc queryex type=service state=all` komutu, Windows işletim sistemindeki servisleri listeler. Bu komut, özellikle Unity geliştiricileri servislerini incelemek ve otomatik görevler oluşturmak için kullanışlıdır. İşte `sc queryex type=service state=all` komutun çeşitli kullanım şekilleri:
* `sc queryex type=service state=all`: Bu temel komut, sistemdeki tüm servisleri listeler.
* `sc queryex type=service state=all | findstr "RUNNING"`: "/findstr" parametresi, sistemdeki tüm servisleri listeler ve "RUNNING" ifadesi içerenlerin sadece adlarını listeler.

![sc_queryex_komutu](https://user-images.githubusercontent.com/69583116/102006562-9 "sc queryex Komutu")

## `wevtutil qe Application /c:10 /f:text` Komutu
`wevtutil qe Application /c:10 /f:text` komutu, Windows işletim sistemindeki uygulama olaylarına bakmak için kullanılır. Bu komut, özellikle Unity geliştiricileri olayları incelemek ve otomatik görevler oluşturmak için kullanışlıdır. İşte `wevtutil qe Application /c:10 /f:text` komutunun çeşitli kullanım şekilleri:
* `wevtutil qe Application /c:10 /f:text`: Bu temel komut, uygulama olaylarını sıralar ve text formatında listeler.
* `wevtutil qe Application /c:10 /f:text | findstr "Unity"`: "/findstr" parametresi, uygulama olaylarını sıralar ve text formatında listeler ve "Unity" ifadesi içerenlerin sadece adlarını listeler.
* `wevtutil qe Application /c:10 /f:text | findstr "Unity" /v`: "/findstr /v" parametresi, uygulama olaylarını sıralar ve text formatında listeler ve "Unity" ifadesi içerenlerin sadece adlarını listeler ve sadece olayları gösterir.

![wevtutil_qe_komutu](https://user-images.githubusercontent.com/69583116/1020065 "wevtutil qe Komutu")

## `netsh wlan show interfaces` Komutu
`netsh wlan show interfaces` komutu, Windows işletim sistemindeki ağlara bakmak için kullanılır. Bu komut, özellikle Unity geliştiricileri ağları incelemek ve otomatik görevler oluşturmak için kullanışlıdır. İşte `netsh wlan show interfaces` komutun çeşitli kullanım şekilleri:
* `netsh wlan show interfaces`: Bu temel komut, sistemdeki tüm ağları listeler.
* `netsh wlan show interfaces | findstr "SSID"`: "/findstr" parametresi, sistemdeki tüm ağları listeler ve "SSID" ifadesi içerenlerin sadece adlarını listeler.
* `netsh wlan show interfaces | findstr "SSID" /v`: "/findstr /v" parametresi, sistemdeki tüm ağları listeler ve "SSID" if adesi içerenlerin sadece adlarını listeler ve sadece ağları gösterir.

![netsh_wlan_show_interfaces_komutu](https://user-images.githubusercontent.com/69583116/102 "netsh wlan show interfaces Komutu")

## `chiper` Komutu
`chiper` komutu, Windows işletim sistemindeki şifrelemeyi kontrol etmek için kullanılır. Bu komut, özellikle Unity geliştiricileri için şifrelemeyi incelemek ve otomatik görevler oluşturmak için kullanışlıdır. İşte `chiper` komutun çeşitli kullanım şekilleri:
* `chiper`: Bu temel komut, şifreleme ile ilgili bilgileri listeler.
* `chiper | findstr "KOD"`: "/findstr" parametresi, şifreleme ile ilgili bilgileri listeler ve "KOD" ifadesi içerenlerin sadece adlarını listeler.
* `chiper | findstr "KOD" /v`: "/findstr /v" parametresi, şifreleme ile ilgili bilgileri listeler ve "KOD" if adesi içerenlerin sadece adlarını listeler ve sadece şifrelemeleri gösterir.
* `chiper /v`: "/v" parametresi, şifreleme ile ilgili bilgileri listeler ve sadece şifrelemeleri gösterir.

![chiper_komutu](https://user-images.githubusercontent.com/69583116/102006563-986 "chiper Komutu")

## `tracert` Komutu
`tracert` komutu, Windows işletim sistemindeki ağlara bakmak için kullanılır. Bu komut, özellikle Unity geliştiricileri ağları incelemek ve otomatik görevler oluşturmak için kullanışlıdır. İşte `tracert` komutun çeşitli kullanım şekilleri:

* `tracert`: Bu temel komut, sistemdeki tüm ağları listeler.
* `tracert | findstr "192.168.1"`: "/findstr" parametresi, sistemdeki tüm ağları listeler ve "192.168.1" ifadesi içerenlerin sadece adlarını listeler.
* `tracert | findstr "192.168.1" /v`: "/findstr /v" parametresi, sistemdeki tüm ağları listeler ve "192.168.1" if adesi içerenlerin sadece adlarını listeler ve sadece ağları gösterir.

![tracert_komutu](https://user-images.githubusercontent.com/69583116/102006564- "tracert Komutu")

## Uyarı
Bu paylaşım Atatürk Üniversitesi Bilişim Sistemleri ve Teknolojileri Bölümü İşletim Sistemleri dersinin ilk vize ödevidir. Sahibi olan Enes Efe Tokta, *6/11/2024-18/11/2024* tarihleri arasında yaptı.