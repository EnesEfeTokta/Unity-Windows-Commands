![unity](Images/WindowsCMDForUnity.png "Unity Windows")

# 🧑‍💻 Unity Geliştiricileri İçin Kullanışlı Windows Komutları 🧑‍💻

## Amaç
Bu dokümanın amacı, Unity geliştiricilerine yönelik olarak Windows işletim sisteminde sıkça kullanılan ve geliştirme sürecini optimize edebilecek komutları kapsamlı bir şekilde sunmaktır. Bu kaynak, geliştiricilerin proje yönetimi, performans izleme ve sistem yapılandırması gibi alanlarda verimliliklerini artırmalarına yardımcı olmayı hedeflemektedir.

## `cd` Komutu ⭐ ⭐
`cd` komutu ile klasörler arasında geçiş yapabiliyoruz. Bu komutun işlevleri şu şekildedir:
*  `cd` komutu ile ilgili klasöre geçiş yapılır.
   ```DOS
   cd <klasör_adı>
   ```
   ![cd_komutu](Images/cd.png "cd Komutu ⭐")

* `cd..` komutu ile bir üst klasörü geçiş yapabiliyoruz. 
   ```DOS
   cd..
   ```

   ![cd_komutu](Images/cd_pointpoint.png "cd.. Komutu ⭐ ⭐")

* `cd.` komutu ile bulunduğumuz klasörü gidebiliyoruz.
   ```DOS
   cd.
   ```
   ![cd_komutu](Images/cd_point.png "cd Komutu ⭐")

* `cd /` komutu ile C: klasörüne gidebiliyoruz.
   ```DOS
   cd /
   ```
   ![cd_komutu](Images/cd_slash.png "cd Komutu ⭐") 

## `mkdir` Komutu ⭐ ⭐
`mkdir` komutu ile klasör oluşturabiliyoruz. Bu komutun işlevleri şu şekildedir:

```DOS
mkdir <klasör_adı>
```

![mkdir_komutu](Images/mkdir.png "mkdir Komutu ⭐")

## `dir` Komutu ⭐ ⭐
`dir` komutu ile klasörlerde bulunan dosyaları ve klasörleri görebiliyoruz. Bu komutun işlevleri şu şekildedir:

* `dir` komutu: Bu, temel `dir` komutudur. Mevcut dizindeki dosyaları ve klasörleri listeler. Gizli dosyaları ve sistem dosyalarını varsayılan olarak göstermez.
   ```DOS
   dir
   ```
   ![dir_komutu](Images/dir.png "dir Komutu ⭐ ⭐")

* `dir /a` komutu: "/a" parametresi "all" (tümü) anlamına gelir. Bu komut, gizli dosyalar ve sistem dosyaları da dahil olmak üzere mevcut dizindeki tüm dosyaları ve klasörleri gösterir.
   ```DOS
   dir /a
   ```
   ![dir_komutu](Images/dir_a.png "dir /a Komutu ⭐ ⭐")

* `dir /a-d` komutu: Bu komut, sadece dosyaları gösterir, klasörleri göstermez. "/a-d" parametresindeki "-d" kısmı "directories" (klasörler) anlamına gelir ve bunları hariç tutar.
   ```DOS
   dir /a-d
   ```
   ![dir_komutu](Images/dir_a_d.png "dir /a-d Komutu ⭐ ⭐")

* `dir /a-h` komutu: Bu komut, gizli olmayan tüm dosyaları ve klasörleri gösterir. "/a-h" parametresindeki "-h" kısmı "hidden" (gizli) anlamına gelir ve gizli dosyaları hariç tutar.
   ```DOS
   dir /a-h
   ```
   ![dir_komutu](Images/dir_a_h.png "dir /a-h Komutu ⭐ ⭐")

Bu komutlar, özellikle Unity projeleri üzerinde çalışırken, proje yapısını incelemek, gizli dosyaları kontrol etmek veya sadece belirli türdeki öğeleri listelemek için kullanışlı olabilir.
* `dir /a-d` komutu ile klasörlerde bulunan dosyaları ve klasörleri görebiliyoruz. 
* `dir /a-h` komutu ile klasörlerde bulunan dosyaları ve klasörleri görebiliyoruz. 

## `copy` Komutu ⭐ ⭐
`copy` komutu ile dosyaları kopyalamak için kullanılır. Bu komutun kullanımı şu şekildedir:

```DOS
copy <kaynak_dosya> <hedef_dosya>
```

![copy_komutu](Images/copy.png "copy Komutu ⭐ ⭐")

## `move` Komutu ⭐ ⭐
`move` komutu ile dosyaları taşımak için kullanılır. Bu komutun kullanımı şu şekildedir:

```DOS
move <kaynak_dosya> <hedef_dosya>
```

![move_komutu](Images/move.png "move Komutu ⭐ ⭐")

## `ipconfig` Komutu ⭐ ⭐
`ipconfig` komutu ile tüm geçerli TCP/IP ağ yapılandırma değerlerini görüntüler ve Dinamik Ana Bilgisayar Yapılandırma Protokolü (DHCP) ve Etki Alanı Adı Sistemi (DNS) ayarlarını yeniler. Parametreler olmadan kullanıldığında, ipconfig tüm bağdaştırıcılar için İnternet Protokolü sürüm 4 (IPv4) ve IPv6 adreslerini, alt ağ maskesini ve varsayılan ağ geçidini görüntüler.

```DOS
ipconfig
```

![ipconfig_komutu](Images/ipconfig.png "ipconfig Komutu ⭐ ⭐")

## `del` Komutu ⭐ ⭐
`del` komutu ile belitririlen dosya silinir. Bu komutun kullanımı şu şekildedir:

```DOS
del <kaynak_yol>
```

![del_komutu](Images/del.png "del Komutu ⭐ ⭐")

## `tasklist` Komutu ⭐ ⭐
`tasklist` komutu ile bilgisayarda çalışan sistemleri listeler.

```DOS
tasklist
```

![tasklist_komutu](Images/tasklist.png "tasklist Komutu ⭐ ⭐")

## `taskkill` Komutu ⭐ ⭐
`taskkill` komutu, Windows'ta çalışan işlemleri (processes) sonlandırmak için kullanılır. Bu komut, özellikle yanıt vermeyen programları kapatmak veya belirli işlemleri sonlandırmak için kullanışlıdır. İşte `taskkill` komutunun çeşitli kullanım şekilleri:

* `taskkill /im <process_name>`: Bu komut, belirtilen isme sahip işlemi nazikçe kapatmaya çalışır. İşlem normal şekilde kapatılır.
   ```DOS
   taskkill /im ⚠️ Notepad.exe
   ```
   ![taskkill_komutu](Images/taskkill_im.png "taskkill /im Komutu ⭐ ⭐")

* `taskkill /f /im <process_name>`: "/f" parametresi "force" (zorla) anlamına gelir. Bu komut, belirtilen işlemi zorla kapatır. İşlem anında sonlandırılır.
   ```DOS
   taskkill /f /im chrome.exe
   ```
   ![taskkill_komutu](Images/taskkill_f_im.png " taskkill /f /im Komutu ⭐")

* `taskkill /f /im <process_name> /t`: "/t" parametresi "tree" (ağaç) anlamına gelir. Bu komut, belirtilen işlemi ve onun başlattığı tüm alt işlemleri zorla kapatır.
   ```DOS
   taskkill /f /im ⚠️ Notepad.exe /t
   ```
   ![taskkill_komutu](Images/taskkill_f_im_t.png "taskkill /f /im /t Komutu ⭐")

* `taskkill /f /pid <process_id> /t`: Bu komut, belirli bir PID'ye sahip işlemi ve onun tüm alt işlemlerini zorla kapatır.
   ```DOS
   taskkill /f /pid 1234 /t
   ```
   ![taskkill_komutu](Images/taskkill_f_pid_t.png "taskkill /f /pid /t Komutu ⭐")

   ⚠️ Not: `process_id` 'yi öğrenmek için, "tasklist" komutunu kullanabilirsiniz.

Bu komutlar, özellikle Unity geliştirme sürecinde yanıt vermeyen Unity uygulamalarını veya editörünü kapatmak, performans sorunlarına neden olan arka plan işlemlerini sonlandırmak veya test amaçlı olarak belirli işlemleri kontrollü bir şekilde kapatmak için kullanışlı olabilir.

⚠️ Not: İşlemleri zorla kapatmak veri kaybına neden olabilir, bu nedenle dikkatli kullanılmalıdır.

## `ping` Komutu ⭐
`ping` komutu ile belirli bir sunucuya bağlanma ve yanıt alma durumlarını kontrol etmek için kullanılır. Bu komutun kullanımı şu şekildedir:
* `ping <sunucu_adresi>`: Bu komut, belirtilen sunucuya bağlanma ve yanıt alma durumlarını kontrol eder
   ```DOS
   ping www.google.com
   ```
   ![ping_komutu](Images/ping.png "ping Komutu ⭐")

* `ping <sunucu_adresi> -t`: Bu komut, belirtilen sunucuya bağlanma ve yanıt alma durumlarını kontrol eder ve her saniye bir kez yanıt alma durumunu kontrol eder.
   ```DOS
   ping www.google.com -t
   ```
   ![ping_komutu](Images/ping_t.png "ping Komutu ⭐")

* `ping <sunucu_adresi> -n <saniye_sayisi>`: Bu komut, belirtilen sunucuya bağlanma ve yanıt alma durumlarını kontrol eder ve belirtilen saniye sayısı kadar yanıt alma durumunu kontrol eder.
   ```DOS
   ping www.google.com -n 10
   ```
   ![ping_komutu](Images/ping_n.png "ping Komutu ⭐")

## `systeminfo` Komutu ⭐
`systeminfo` komutu ile bilgisayarın bilgilerini görüntüler. Bu komutun kullanımı şu şekildedir:
* `systeminfo`: Bu komut, bilgisayarın işletim sistemi, işlemci, ana bilgisayar, kullanıcı, sürücü ve disk bilgisini, görüntüsü ve bağlantı bilgilerini görüntüler.
   ```DOS
   systeminfo
   ```
   ![systeminfo_komutu](Images/systeminfo.png "systeminfo Komutu ⭐")

* `systeminfo /fo csv`: Bu komut, bilgisayarın işletim sistemi, işlemci, ana bilgisayar, kullanıcı, sürücü ve disk bilgisini, csv (comma-separated values) biçiminde görüntüler.
   ```DOS
   systeminfo /fo csv
   ```
   ![systeminfo_komutu](Images/systeminfo_fo_csv.png "systeminfo Komutu ⭐")

* `systeminfo /fo list`: Bu komut, bilgisayarın işletim sistemi, işlemci, ana bilgisayar, kullanıcı, sürücü ve disk bilgisini, listeleri (table) biçiminde görüntüler.
   ```DOS
   systeminfo /fo list
   ```
   ![systeminfo_komutu](Images/systeminfo_fo_l.png "systeminfo Komutu ⭐")

## `tree` Komutu ⭐
`tree` komutu, bir dizinin yapısını görsel olarak gösteren kullanışlı bir Windows komutudur. Bu komut, özellikle karmaşık proje yapılarına sahip Unity projelerinde dosya ve klasör hiyerarşisini anlamak için çok faydalı olabilir. İşte `tree` komutunun çeşitli kullanım şekilleri:

* `tree <dizin_yolu>`: Bu temel komut, belirtilen dizinin alt dizinlerini ve klasör yapısını gösterir. Dosyaları göstermez.
   ```DOS
   tree C:\UnityProjects\MyGame
   ```
   ![tree_komutu](Images/tree.png "tree Komutu ⭐")

* `tree <dizin_yolu> /f`: "/f" parametresi "files" (dosyalar) anlamına gelir. Bu komut, dizin yapısını gösterirken her klasördeki dosyaları da listeler.
   ```DOS
   tree C:\UnityProjects\MyGame /f
   ```
   ![tree_komutu](Images/tree_f.png "tree /f Komutu ⭐")

   ⚠️ Not 1: Çıktının uzunluğu fazla olabilir. O yüzden dikkatli olun.
   
   ⚠️ Not 2: Çıktının uzunluğu fazla olduğu için ekranda ufak bir bir bölümü gösteridim.

* `tree <dizin_yolu> /a`: "/a" parametresi "ASCII" anlamına gelir. Bu komut, dizin yapısını gösterirken ASCII karakterleri kullanır. Bu, özellikle çıktıyı bir metin dosyasına yönlendirirken veya bazı konsolların grafik karakterleri düzgün göstermediği durumlarda faydalıdır.
   ```DOS
   tree C:\UnityProjects\MyGame /a
   ```
   ![tree_komutu](Images/tree_a.png "tree /a Komutu ⭐")

   ⚠️ Not: Çıktının uzunluğu fazla olduğu için ekranda ufak bir bir bölümü gösteridim.

* `tree <dizin_yolu> /a /f`: Bu komut, ASCII karakterleri kullanarak hem dizin yapısını hem de dosyaları gösterir.
   ```DOS
   tree C:\UnityProjects\MyGame /a /f
   ```
   ![tree_komutu](Images/tree_a_f.png "tree /a /f Komutu ⭐")

   ⚠️ Not: Çıktının uzunluğu fazla olduğu için ekranda ufak bir bir bölümü gösteridim.

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

⚠️ Not: Çok büyük projelerde `/f` parametresini kullanırken dikkatli olun, çünkü çıktı oldukça uzun olabilir.

## `perfmon /report` Komutu ⭐
`perfmon /report` komutu, performans izleyicisini açar. Cihazın performansını ölçülmesine olanak sağlar.
```DOS
perfmon /report
```
![perfmon_komutu](Images/perfmon_report.png "perfmon /report Komutu")

## `nvidia-smi` Komutu ⭐
`nvidia-smi` komutu, NVIDIA grafik kartınız varsa, bu komut ile GPU'nuzun performansını, sıcaklığını ve kullanım oranını görebilirsiniz.

⚠️ Not: Bu komutun çalışması için NVIDIA grafik kartınızın olması gerekli.

![nvidia-smi_komutu](Images/nvidia_smi.png "nvidia-smi Komutu")

## `type` Komutu ⭐
 `type` komutu, bir dosya veya metin dosyasının içeriğini görmek için kullanılır. Bu komut, özellikle bir metin dosyasının içeriğini görmek için kullanışlıdır. İşte `tyepe` komutunun kullanım örneği:
 ```DOS
 type C:\UnityProjects\MyGame\Assets\Scripts\MyScript.cs
 ```
 ![type_komutu](Images/type.png "type Komutu ⭐")

 ## `findstr` Komutu ⭐
 `findstr` komutu, bir dosyada belirtilen kelimeyi bulmak için kullanılır. Bu komut, özellikle metin dosyalarında arama yapmak için kullanışlıdır. İşte `findstr` komutunun kullanım örneği:
 ```DOS
 findstr "Hello" C:\UnityProjects\MyGame\Assets\Scripts\MyScript.cs
 ```
 ![findstr_komutu](Images/findstr.png "findstr Komutu ⭐")

## `driverquery` Komutu ⭐
`driverquery` komutu, Windows işletim sisteminde yüklü olan sürücülerin (drivers) listesini görüntülemek için kullanılır. Bu komut, özellikle Unity geliştiricileri için donanım uyumluluğu ve performans sorunlarını teşhis etmede yararlı olabilir. İşte `driverquery` komutunun çeşitli kullanım şekilleri:

* `driverquery`: Bu temel komut, sistemde yüklü olan tüm sürücülerin basit bir listesini gösterir.
   ```DOS
   driverquery
   ```
   ![driverquery_komutu](Images/driverquery.png "driverquery Komutu ⭐")

* `driverquery /v`: "/v" parametresi "verbose" (ayrıntılı) anlamına gelir. Bu komut, sürücüler hakkında daha detaylı bilgi sağlar, örneğin sürücü sağlayıcısı, sürücü versiyonu ve sürücü türü gibi.
   ```DOS
   driverquery /v
   ```
   ![driverquery_komutu](Images/driverquery_v.png "driverquery /v Komutu ⭐")

* `driverquery /fo csv`: "/fo csv" parametresi, çıktıyı CSV (Comma-Separated Values) formatında oluşturur. Bu, sürücü bilgilerini Excel gibi bir uygulamada analiz etmek isteyenler için kullanışlıdır.
   ```DOS
   driverquery /fo csv > drivers.csv
   ```
   ![driverquery_komutu](Images/driverquery_fo_csv.png "driverquery /fo csv Komutu ⭐")

* `driverquery /si`: "/si" parametresi "signed" (imzalı) anlamına gelir. Bu komut, dijital olarak imzalanmış sürücüler hakkında bilgi verir, ki bu güvenlik açısından önemlidir.
   ```DOS
   driverquery /si
   ```
   ![driverquery_komutu](Images/driverquery_si.png "driverquery /si Komutu ⭐")

Unity geliştiricileri için `driverquery` komutunun kullanım örnekleri:

1. Grafik sürücülerini kontrol etmek:
   `driverquery | findstr "NVIDIA"`
   ```DOS
   driverquery | findstr "NVIDIA"
   ```
   ![driverquery_komutu](Images/driverquery_nvidia.png "driverquery /si Komutu ⭐")

   ⚠️ Not: `findstr` komutu, parametre olarak verilen yeri kendi cihazınıza göre değiştiriniz. Bu görselde Nvidia işletim sisteminde sürücülerin yüklü olduğunu görüyorsunuz.

2. Ses sürücülerini incelemek:
   `driverquery | findstr "audio"`
   ```DOS
   driverquery | findstr "audio"
   ```
   ![driverquery_komutu](Images/driverquery_audio.png "driverquery /si Komutu ⭐")

3. Tüm sürücüleri ayrıntılı bir şekilde bir CSV dosyasına kaydetmek:
   `driverquery /v /fo csv > unity_system_drivers.csv`
   ```DOS
   driverquery /v /fo csv > unity_system_drivers.csv
   ```
   ![driverquery_komutu](Images/driverquery_v_fo_csv.png "driverquery /v /fo csv Komutu ⭐")

4. İmzalanmamış sürücüleri tespit etmek (potansiyel güvenlik riskleri):
   `driverquery /si | findstr "FALSE"`
   ```DOS
   driverquery /si | findstr "FALSE"
   ```
   ![driverquery_komutu](Images/driverquery_si_false.png "driverquery /si Komutu ⭐")

Bu komut, Unity projelerinde performans sorunları yaşandığında, özellikle grafik veya ses ile ilgili problemlerde, sistemdeki sürücülerin durumunu kontrol etmek için kullanılabilir. Ayrıca, farklı test ortamları arasında sürücü uyumluluğunu karşılaştırmak için de faydalıdır.

⚠️ Not: Sürücülerle ilgili herhangi bir değişiklik yapmadan önce, sistem yedeği almak ve dikkatli olmak önemlidir.

## `getmac` Komutu ⭐
`getmac` komutu, Windows işletim sistemindeki MAC adresini (Media Access Control) görüntüler. Bu komut, özellikle Unity geliştiricileri mac adreslerini, dizinleri ve diğer bağlantıları kontrol etmek için kullanışlıdır. İşte `getmac` komutunun çeş itli kullanım şekilleri:

* `getmac`: Bu temel komut, sistemdeki herhangi bir MAC adresini görüntüler.
   ```DOS
   getmac
   ```
   ![getmac_komutu](Images/getmac.png "getmac Komutu ⭐")

* `getmac /fo table /nh /v`: "/all" parametresi, sistemdeki tüm MAC adreslerini görüntüler.
   ```DOS
   getmac /fo table /nh /v
   ```
   ![getmac_komutu](Images/getmac_fo_table_nh_v.png "getmac /all Komutu ⭐")

## `powercfg` Komutu ⭐
`powercfg` komutu, Windows işletim sistemindeki performans ve güvenlik ayarlarını yönetmek için kullanılır. Bu komut, özellikle Unity geliştiricileri performans ve güvenlik ayarlarını değiştirmek için kullanışlıdır. İşte `powercfg` komutunun çeşitli kullanı şekilleri:

* `powercfg`: Bu temel komut, sistemdeki tüm performans ve güvenlik ayarlarını listeler.
   ```DOS
   powercfg
   ```
   ![powercfg_komutu](Images/powercfg.png "powercfg Komutu ⭐")

* `powercfg /a`: "/a" parametresi, sistemdeki tüm performans ayarlarını listeler.
   ```DOS
   powercfg /a
   ```
   ![powercfg_komutu](Images/powercfg_a.png "powercfg /a Komutu ⭐")

* `powercfg /q`: "/q" parametresi, sistemdeki tüm güvenlik ayarlarını listeler.
   ```DOS
   powercfg /q
   ```
   ![powercfg_komutu](Images/powercfg_q.png "powercfg /q Komutu ⭐")

* `powercfg /batteryreport`: "/batteryreport" parametresi, batarya raporunu görüntüler ve bilgisyara kaydedir.
   ```DOS
   powercfg /batteryreport
   ```
   ![powercfg_komutu](Images/powercfg_batteryreport.png "powercfg /batteryreport Komutu ⭐")

## `xcopy /s /i "Dosya_Yol" "Dosya_Yol"` Komutu ⭐
`Xcopy` komutu, Windows işletim sistemindeki dosyaları ve dizinleri kopyalamak için kullanılır. Bu komut, özellikle Unity geliştiricileri içeri aktarmak için kullanışlıdır. İşte `xcopy` komutunun çeşitli kullanı şekli:
```DOS
xcopy /s /i "Dosya_Yol" "Dosya_Yol"
```
![xcopy_komutu](Images/xcopy_s_i.png "xcopy /s /i Komutu ⭐")

## `wmic` Komutu ⭐
`wmic` (Windows Management Instrumentation Command-line) komutu, Windows sistemlerinde sistem yönetimi ve bilgi toplama için güçlü bir araçtır. Unity geliştiricileri için, özellikle donanım bilgilerini toplamak, sistem durumunu kontrol etmek ve otomatik görevler oluşturmak için kullanışlıdır. İşte `wmic` komutunun Unity geliştiricileri için önemli kullanım örnekleri:

1. Sistem Bilgilerini Almak:
   * `wmic computersystem get model,name,manufacturer,systemtype`: Bilgisayarın modelini, adını, üreticisini ve sistem türünü gösterir.
      ```DOS
      wmic computersystem get model,name,manufacturer,systemtype
      ```
      ![wmic_komutu](Images/wmic_computersystem.png "wmic computersystem Komutu ⭐")

   * `wmic os get caption,version,osarchitecture`: İşletim sistemi adını, sürümünü ve mimarisini gösterir.
      ```DOS	
      wmic os get caption,version,osarchitecture
      ```
      ![wmic_komutu](Images/wmic_os_get_caption_version_osarchitecture.png "wmic os get caption,version,osarchitecture Komutu ⭐")

2. Donanım Bilgilerini Kontrol Etmek:
   * `wmic cpu get name,numberofcores,maxclockspeed`: İşlemci adını, çekirdek sayısını ve maksimum hızını gösterir.
      ```DOS
      wmic cpu get name,numberofcores,maxclockspeed
      ```
      ![wmic_komutu](Images/wmic_cpu_get_name_numberofcores_maxclockspeed.png "wmic cpu get name,numberofcores,maxclockspeed Komutu ⭐")

   * `wmic memorychip get capacity,speed`: RAM kapasitesini ve hızını gösterir.
      ```DOS
      wmic memorychip get capacity,speed
      ```
      ![wmic_komutu](Images/wmic_memorychip_get_capacity_speed.png "wmic memorychip get capacity,speed Komutu ⭐")

   * `wmic diskdrive get model,size,status`: Sabit disk modelini, boyutunu ve durumunu gösterir.
      ```DOS	
      wmic diskdrive get model,size,status
      ```
      ![wmic_komutu](Images/wmic_diskdrive_get_model_size_status.png "wmic diskdrive get model,size,status Komutu ⭐")

3. Grafik Kartı Bilgilerini Almak:
   * `wmic path win32_VideoController get name,adapterram,driverversion`: Grafik kartı adını, RAM'ini ve sürücü sürümünü gösterir.
      ```DOS
      wmic path win32_VideoController get name,adapterram,driverversion
      ```
      ![wmic_komutu](Images/wmic_path_win32_VideoController_get_name_adapterram_driverversion.png "wmic path win32_VideoController get name,adapterram,driverversion Komutu ⭐")

4. Çalışan Uygulamaları Listelemek:
   * `wmic process where "name like '%Unity%'" get name,processid,commandline`: Çalışan Unity ile ilgili süreçleri listeler.
      ```DOS
      wmic process where "name like '%Unity%'" get name,processid,commandline
      ```
      ![wmic_komutu](Images/wmic_process_where_name_like_Unity_get_name_processid_commandline.png "wmic process where name like '%Unity%' get name,processid,commandline Komutu ⭐")

      ⚠️ Not: Çıktının uzunluğu fazla olduğu için çıktının bir kısmını göstermekteyim.

5. Sistem Performansını İzlemek:
   * `wmic cpu get loadpercentage`: CPU kullanım yüzdesini gösterir.
      ```DOS
      wmic cpu get loadpercentage
      ```
      ![wmic_komutu](Images/wmic_cpu_get_loadpercentage.png "wmic cpu get loadpercentage Komutu ⭐")

   * `wmic memorychip get capacity`: Toplam RAM kapasitesini gösterir.
      ```DOS
      wmic memorychip get capacity
      ```
      ![wmic_komutu](Images/wmic_memorychip_get_capacity.png "wmic memorychip get capacity Komutu ⭐")

6. Unity Projesi için Otomatik Görevler:
   * `wmic process call create "C:\Program Files\Unity\Hub\Editor\2021.3.0f1\Editor\Unity.exe -projectPath C:\UnityProjects\MyGame -batchmode -quit -logFile C:\buildlog.txt -buildWindows64Player C:\Builds\MyGame.exe"`: Unity projesini komut satırından derler.
      ```DOS	
      wmic process call create wmic process call create "C:\Program Files\Unity\Hub\Editor\2021.3.0f1\Editor\Unity.exe -projectPath C:\UnityProjects\MyGame -batchmode -quit -logFile C:\buildlog.txt -buildWindows64Player C:\Builds\MyGame.exe"
      ```

7. Sistem Günlüklerini İncelemek:
   * `wmic nteventlog get path,filename,writedate`: Sistem olay günlüklerini listeler.
      ```DOS
      wmic nteventlog get path,filename,writedate
      ```
      ![wmic_komutu](Images/wmic_nteventlog_get_path_filename_writedate.png "wmic nteventlog get path filename writedate Komutu ⭐")

Bu komutlar, Unity geliştiricilerinin sistem durumunu analiz etmelerine, performans sorunlarını teşhis etmelerine ve otomatik derleme süreçleri oluşturmalarına yardımcı olabilir. Ayrıca, farklı test ortamlarında tutarlı sistem bilgileri toplamak için de kullanışlıdır.

⚠️ Not: Bazı `wmic` komutları yönetici ayrıcalıkları gerektirebilir. Ayrıca, Microsoft Windows 11'de `wmic` yerine daha modern `Get-WmiObject` PowerDOS cmdlet'i kullanılması önerilmektedir.

## `sc queryex type=service state=all` Komutu ⭐
`sc queryex type=service state=all` komutu, Windows işletim sistemindeki servisleri listeler. Bu komut, özellikle Unity geliştiricileri servislerini incelemek ve otomatik görevler oluşturmak için kullanışlıdır. İşte `sc queryex type=service state=all` komutun çeşitli kullanım şekilleri:
* `sc queryex type=service state=all`: Bu temel komut, sistemdeki tüm servisleri listeler.
   ```DOS	
   sc queryex type=service state=all
   ```
   ![sc_queryex_komutu](Images/sc_queryex_type_service_state_all.png "sc queryex Komutu ⭐")

* `sc queryex type=service state=all | findstr "RUNNING"`: "/findstr" parametresi, sistemdeki tüm servisleri listeler ve "RUNNING" ifadesi içerenlerin sadece adlarını listeler.
   ```DOS   
   sc queryex type=service state=all | findstr "RUNNING"
   ```
   ![sc_queryex_komutu](Images/sc_queryex_type_service_state_all_findstr_running.png "sc queryex Komutu ⭐")

## `wevtutil qe Application /c:10 /f:text` Komutu ⭐
`wevtutil qe Application /c:10 /f:text` komutu, Windows işletim sistemindeki uygulama olaylarına bakmak için kullanılır. Bu komut, özellikle Unity geliştiricileri olayları incelemek ve otomatik görevler oluşturmak için kullanışlıdır. İşte `wevtutil qe Application /c:10 /f:text` komutunun çeşitli kullanım şekilleri:
* `wevtutil qe Application /c:10 /f:text`: Bu temel komut, uygulama olaylarını sıralar ve text formatında listeler.
   ```DOS	
   wevtutil qe Application /c:10 /f:text
   ```
   ![wevtutil_qe_komutu](Images/wevtutil_qe_Application_c_10_f_text.png "wevtutil qe Komutu ⭐")

* `wevtutil qe Application /c:10 /f:text | findstr "Unity"`: "/findstr" parametresi, uygulama olaylarını sıralar ve text formatında listeler ve "Unity" ifadesi içerenlerin sadece adlarını listeler.
   ```DOS		
   wevtutil qe Application /c:10 /f:text | findstr "Unity"
   ```

   ![wevtutil_qe_komutu](Images/wevtutil_qe_Application_c_10_f_text_findstr_Unity.png "we_qe_Application_c_10_f_text_findstr_Unity.png wevtutil qe Komutu ⭐")

* `wevtutil qe Application /c:10 /f:text | findstr "Unity" /v`: "/findstr /v" parametresi, uygulama olaylarını sıralar ve text formatında listeler ve "Unity" ifadesi içerenlerin sadece adlarını listeler ve sadece olayları gösterir.
   ```DOS
   wevtutil qe Application /c:10 /f:text | findstr "Unity" /v
   ```
   ![wevtutil_qe_komutu](Images/wevtutil_qe_Application_c_10_f_text.png "wevtutil qe Komutu ⭐")

## `netsh wlan show interfaces` Komutu ⭐
`netsh wlan show interfaces` komutu, Windows işletim sistemindeki ağlara bakmak için kullanılır. Bu komut, özellikle Unity geliştiricileri ağları incelemek ve otomatik görevler oluşturmak için kullanışlıdır. İşte `netsh wlan show interfaces` komutun çeşitli kullanım şekilleri:
* `netsh wlan show interfaces`: Bu temel komut, sistemdeki tüm ağları listeler.
   ```DOS	
   netsh wlan show interfaces
   ```
   ![netsh_wlan_show_interfaces_komutu](Images/netsh_wlan_show_interfaces.png "netsh wlan show interfaces Komutu ⭐")

* `netsh wlan show interfaces | findstr "SSID"`: "/findstr" parametresi, sistemdeki tüm ağları listeler ve "SSID" ifadesi içerenlerin sadece adlarını listeler.
   ```DOS	
   netsh wlan show interfaces | findstr "SSID"
   ```
   ![netsh_wlan_show_interfaces_komutu](Images/netsh_wlan_show_interfaces_findstr_SSID.png "netsh wlan show interfaces findstr SSID Komutu ⭐")

* `netsh wlan show interfaces | findstr "SSID" /v`: "/findstr /v" parametresi, sistemdeki tüm ağları listeler ve "SSID" if adesi içerenlerin sadece adlarını listeler ve sadece ağları gösterir.
   ```DOS
   netsh wlan show interfaces | findstr "SSID" /v
   ```
   ![netsh_wlan_show_interfaces_komutu](Images/netsh_wlan_show_interfaces_findstr_SSID_v.png "netsh wlan show interfaces findstr SSID /v Komutu ⭐")

## `nslookup` Komutu ⭐
`nslookup` komutu, belirli bir web sitesinin veya etki alanının IP adresini bulmak için "nslookup" komutunu kullanabilirsiniz. İşte `nslookup` komutunun çeşitli kullanım şekili:
`nslookup`: Bu temel komut, sistemdeki tüm ağları listeler.
```DOS
nslookup
```
![nslookup_komutu](Images/nslookup.png "nslookup Komutu ⭐")

## `tracert` Komutu ⭐
`tracert` komutu, Windows işletim sistemindeki ağlara bakmak için kullanılır. Bu komut, özellikle Unity geliştiricileri ağları incelemek ve otomatik görevler oluşturmak için kullanışlıdır. İşte `tracert` komutun çeşitli kullanım şekilleri:

* `tracert`: Bu temel komut, sistemdeki tüm ağları listeler.
   ```DOS
   tracert
   ```
   ![tracert_komutu](Images/tracert.png "tracert Komutu ⭐")

* `tracert | findstr "192.168.1"`: "/findstr" parametresi, sistemdeki tüm ağları listeler ve "192.168.1" ifadesi içerenlerin sadece adlarını listeler.
   ```DOS
   tracert | findstr "192.168.1"
   ```
   ![tracert_komutu](Images/tracert_findstr_192_168_1.png "tracert | findstr 192.168.1 Komutu ⭐")

## İletişim
* [LinkedIn](https://www.linkedin.com/in/enes-efe-tokta/ "Click on Enes Efe Tokta's LikedIn connection link.")
* [GitHub](https://github.com/EnesEfeTokta "Enes Efe Tokta's Github profile.")
* [Email](enesefetokta009@gamil.com  "Click on Enes Efe Tokta's Email.")

## Proje Bilgileri
Bu doküman, Atatürk Üniversitesi Bilişim Sistemleri ve Teknolojileri Bölümü'nde yürütülen İşletim Sistemleri dersi kapsamında hazırlanmış bir akademik çalışmadır. Projenin geliştiricisi Enes Efe Tokta tarafından *6 Kasım 2024* ile *18 Kasım 2024* tarihleri arasında titizlikle hazırlanmış ve dersin ilk ara sınav ödevi olarak sunulmuştur.

Bu çalışma, Windows işletim sistemi komutlarını Unity geliştirme ortamı bağlamında incelemekte ve açıklamaktadır. Doküman, hem akademik hem de pratik amaçlara hizmet etmek üzere tasarlanmıştır.

© 2024 Enes Efe Tokta. Tüm hakları saklıdır. [LICENSE](https://github.com/EnesEfeTokta/Unity-Windows-Commands/blob/main/LICENSE "Click on LICENSE file.")