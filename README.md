<img align="left" src="https://user-images.githubusercontent.com/25962055/80995892-a4fba980-8e47-11ea-81b6-ddbf19882fab.png" height="120" width="100">

# Linux sık kullandığım komutlar silsilesi <br/>
<br/>

Linux tabanlı işletim sistemlerini çoğunlukla terminal üzerinden kontrol edilmektedir.
Linux, GNU standardında açık kaynak kodlu, özgür yazılım olduğundan çeşitli geliştiriciler tarafından farklı komutlar geliştirilmiştir.
Bu komutlar disk işlemleri, ağ işlemleri, dosya paylaşım işlemleri vb. gruplara ayrılabilir.

shell **::** kabuk **::** çeşitli shell’ler **::** bash, csh, zsh <br/>
Kullanıcı **<=>** Shell **<=>** İşletim Sistemi **<=>** Donanım <br/>

directory : **dizin** <br/>
~ : tilde : **kullanıcı dizini** : home directory <br/>
/ : **root dizini** <br/>
root : **kök** <br/>
prompt : **komut yazdığım yer** <br/>

cd **- change directory** <br/>
cd / : **Dizinler arası geçiş için kullanılır. Ana dizine gider.** <br/>
cd ~ : **Kullanıcı ev dizinine gider.** <br/>
cd : **sadece komut yazılırsa da ev dizinine gider.** <br/>
cd .. : **üst dizine gider.** <br/>
cd /etc : **Kök dizinindeki etc dizinine gider** <br/>

pwd - **print work directory** <br/>
pwd : **mevcut dizin yolunu kök dizinden itibaren tam yolunu verir.** <br/>

ls - **list directory - Dizin ve dosyaları listelemek için kullanılır.** <br/>
ls : **Bulunduğun dizin ve dosyaları listeler.** <br/>
ls -a : **gizli dizin dosyalarını listeler.** <br/>
ls -l : **dizin ve dosyaları detaylı olarak listeler.** <br/>
ls -lh : **dizin ve dosya boyutlarını okunabilir biçimde listeler.** <br/>
ls dizinimiz : **Komuta dizin seçeneği verilirse, verilen dizin listelenir.** <br/>
ls / -l : **Kök dizineki dizin ve dosyaları liste biçiminde listeler.** <br/>
ls -d parametremiz : **Sadece dizinleri listelemek için.** <br/>
ls -lah : **Genel kullanımı** <br/>
ls -tl : **zamana göre sırala** <br/>
ls -alt : **gizli dosyalarda dahil** <br/>
ls -altr : **zamanıda tersine çeviriyor** <br/>
ls -Sl : **boyutuna göre sırala** <br/>
ls -rSl : **tersten sırala** <br/>
ls - rSla : **gizli dosyalarıda dahil et** <br/>
ls -Slrh : **size’ları düzeltti** <br/>

cat - **concatenate files** <br/>
cat metin.txt : **dosya içeriğini okumak için kullanılır.** <br/>
cat -n metin.txt : **dosya içeriğini numaralandırmak için n kullanılır.** <br/>
cat > dosyamız : **Ayrıca dosya oluşturmak içinde kullanılır.** <br/>

touch metin.txt : **genellikle tablo oluşturmak için kullanılır.** <br/>

clear : **terminal ekranını temizler** <br/>

service : **Çalışan servislerle ilgili işlem yapmak için kullanılır.** <br/>
service servisimiz start : **Servisi başlatmak için start kullanılır.** <br/>
service servisimiz status : **Servis hakkında bilgi almak için status kullanırlı.** <br/>
service servisimiz restart : **Yeniden başlatmak için.** <br/>
service servisimiz reload : **Ayarları yeniden yüklemek için.** <br/>
service servisimiz stop : **Durdurmak için.** <br/>

top : **Çalışan uygulamaların hafıza, işlemci vb. kullanım bilgilerini verir.** <br/>
top -c : **İşlemci kullanımna göre sıralamak için.** <br/>

ping www.google.com : **Uzak sistemi sorgulamak için kullanılır.** <br/>
uptime : **Sistemin çalışma zamanını verir.** <br/>
whoami : **Mevcut kullanıcı bilgilerini verir.** <br/>
whereis : **Genellikle uygulama ayar dosyalarını hızlıca bulmak için kullanılır.** <br/>
poweroff : **Sistemi kapatır** <br/>
whatis poweroff: **Komutlarla ilgili kısa bilgi almak için kullanılır.** <br/>
man ls : **komutlarla ilgili detaylı bilgi almak için kullanılır.** <br/>

mkdir - **make directory** <br/>
mkdir <dizin_adi> : **Dizin oluşturmak için kullanılır.** <br/>
mkdir <dizin_adi> <dizin_adi2> <dizin_adi3> : **Birden fazla.** <br/>
mkdir -p <dizin_adi/dizin_adi2/dizin_adi3> : **Dizin altında oluşturmak için.** <br/>
mkdir -pv <dizin_adi/dizin_adi2/dizin_adi3> : **İşlem sonucuyla ilgili bilgi almak için.** <br/>

rmdir - **remove directory** <br/>
rmdir <dizin_adi> : **Boş dizin silme işleminde kullanılır.** <br/>

rm : remove : **dizinleri içindekilerle birlikte silmek için kullanılır** <br/>
rm -rf <dizin_adi> : **Dosya veya dizin silme işlemi için kullanılır.** <br/>
**Kullanırken dikkatli olmakta fayda var.** <br/>
sudo rm -rf dizin : **dizin ve altındakileri sil** <br/>

**Eğer sadece dizini silmek istiyorsanız, rmdir’e bir alternatif olarak rm -r kullanın.** <br/>
rm -i deneme.html : **ben bu dosyayı kaldırayım mı diye soruyor emin misin?** <br/>

rm -d test : **test dizinini sil : boşsa siler** <br/>
rm -r dizin1 : **içi dolu olsada sildi** <br/>

cp - **copy** <br/>
cp -r kaynak hedef : **dosya veya dizin kopyalama için kullanılır.** <br/>
cp -r kaynak kaynak1 kaynak2 hedef : **Birden fazla kopyalama.** <br/>

md - **move** <br/>
mv kaynak hedef : **Dosya veya dizin taşımak için kullanılır.** <br/>
mc dizin yeni_dizin_adi : **Dosya veya dizin adını değiştirmek içinde kullanılabilir.** <br/>

du
du -sh dizin : **Dizin boyutunu öğrenmek için kullanılır.**
du -sh * : **Dizin içerisindeki tüm dizinlerin boyutunu öğrenmek için kullanılır.**
du -shc * : **Dizinlerin toplam boyutu için c parametresi kullanılabilir.**

find <br/>
find <aranacak_yer> -type d -name <dizin_adi> : **Dosya ve dizin aramak için kullanılır.** <br/>
find arama_yeri -name aranan : **Geniş bir kullanımı olan arama komutu.** <br/>
find arama_yeri -iname aranan : **Aramayı büyük küçük harfe duyarsız olarak yapmak için iname parametresi kullanılır.** <br/>
find <arama_yeri> -name <ara*> : **Tam adı bilinmiyorsa yıldır karakteri kullanılır.** <br/>
find <arama_yeri> -name <*.txt> : **Örneğin uzantısı .txt olan dosyaları bulmak için aşağıdaki komut kullanılabilri.** <br/>

find -type d aranan : **Parametre d alırsa dizin, f alırsa dosyaları listeler.** <br/>
find <arama_yeri> -name <aranan> -size +10k : Aranan ifadenin boyutunu belirtmek için size parametresi kullanılır. <br/>
  
head dosya : **Dosya içeriğini dosya başından itibaren okumak için kullanılır.** <br/>
head -n3 dosya : **Satır sayısını belirtmek için n parametresi kullanılır.** <br/>
head -c3 dosya : **Karakter sayısını belirtmek için c parametresi kullanılır.** <br/>

tail  dosya : **Dosya içeriğini dosya sonundan itibaren okumak için kullanılır. (Varsayılan 10 satır)** <br/>
tail -n3 dosya : **Satır sayısını belirtmek için n parametresi kullanılır.** <br/>
tail -c3 dosya : **Karakter sayısını belirtmek için c parametresi kullanılır.** <br/>
tail -f dosya : **Dosya değişikliklerini takip etmek için f parametresi kullanılır.** <br/>

more dosya : **Dosya içeriğini parça parça okumak için kullanılır.** <br/>
less dosya : **Dosya içeriğini more komutundan daha fazla seçenekler parça parça okumak için kullanılır.** <br/>

sort dosya : **Dosya içeriğini sıralı okumak için kullanılır.** <br/>
nl dosya : **Dosya içeriğini satır numarası ekleyerek okuma yapar.** <br/>
pr dosya : **Dosya içeriğini sayfalayarak okumak için kullanılır.** <br/>
tee dosya : **Yeni bir komut oluşturmak ve çıktı yönlendirme.** <br/>
file dosya : **Dosya ile ilgili bilgi almak için kullanılır.** <br/>
stat dosya : **Dosya ile ilgili detaylı bili** <br/>

whereis ve which - **Çalıştırılabilir dosyaların konumunu bulmak için kullanılır.** <br/> 
whereis <komut> <br/>
whereis cd <br/>
which <komut> <br/>
which cd <br/>
  
grep aranan dosya : **Arama yapmak için kullanılır** <br/> 
grep -i aranan dosya : **Bütük küçük harfe duyarlı** <br/> 
grep -r aranan dizin : **Aramayı dizin altındaki tüm dosya ve dizinlerde yapmak için r parametresi kullanılır.** <br/> 
grep -ir '^Merhaba' dosya.txt  : **Arama sırasında başlangıç(^) ve bitiş ($) karakterleri ile arama yapılabilir** <br/> 

**ÇIKTI YÖNLENDİRME <br/> 
Çalıştırılan komutların sonuçlarını bir dosya yazdırmak veya eklemek için çıktı yönlendirme kullanılır. <br/> 
Linux komutları temel olarak 3 farklı tanımlayıcıya sahiptir.** <br/> 
Standart girdi(stdin)< - Komuta girdi olarak kullanılır. <br/> 
  
komut < dosya <br/> 

Standart çıktı (stdout) > - **Komut sonucu çıktı olarak kulanılır.** <br/> 
komut > dosya <br/> 
 
**Dosya ve dizinleri dosyaya kaydetmek için;** <br/> 
ls -lah > liste.txt <br/> 

**Dosya üzerine ekleme yapmak için çift yönlendirme (>>) kullanılabilir.** <br/> 
komut >> mevcut_dosya <br/> 

**Dosya ve dizinlerin dosya üzerine kaydetmek için;** <br/> 
ls -lah >> liste.txt <br/> 

**Standart hata (stdorr) 2> - Komut hatası çıktı olarak kullanılır.** <br/> 
hatali_komut 2> dosya <br/> 

**Komut hatasını dosyaya kaydetmek için;** <br/> 
hatali_komut 2> hata.txt <br/> 

**ARDIŞIK KOMUTLAR <br/> 
Bir komutun sonucunu başka bir komuta kullanmak için ardışık komutlar | kullanılır. <br/> 
Genellikle komut çıktısında arama yapmak için kullanılır..** <br/> 

**Listeleme komutunun sonucu grep komutuna gönderilerek komut sonucunda arama yapılır.** <br/> 
ls -lah | grep '^d' <br/> 

**Çalışan işlemler çıktısı wc komutuna gönderilerek çalışan işlem sayısı bulunmuştur.** <br/> 
ps -aux | wc -l <br/> 

**Uzun komut sonuçlarını parça parça okumak için more ve less komutuna yönlendirme de sıklıkla kullanılır.** <br/> 
ls -lah | more <br/> 
ls -lah | less <br/> 

**Bağlı Komutlar** <br/> 
**Bir komutun çalışma durumuna göre sonraki komutun çalışması için bağlı komutlar (&&) kullanılır.** <br/> 
make && make install <br/> 
**Birinci komut çalışmadığında ikinci komut çalışmayacaktır.** <br/> 

**Sıralı Komutlar** <br/> 
komut; komut1; komut2 Komutları sırayla çalıştırmak için sıralı komutlar (;) kullanılır. <br/> 
pwd;ls -lah <br/> 
pwd;ls -lah;date <br/> 

**Linux Dosya ve Dizin İzinleri** <br/>
**Linux’ta her şey bir dosya olduğundan dosya ve dizin izinleri önemlidir.** <br/>
ls -l : **Dosya ve dizin izinlerini öğrenmek için ls komutu ve l parametresi kullanılır.** <br/>
stat -c "%a %n" * : **Diğer bir yöntemle stat komutunun kullanılmasıdır.** <br/>

**İzin bölümündeki ilk harf dosya tipini, diğerleri ise izinleri ifade eder.** <br/>
**Dosya tipi harfi d ise dizin, tire (-) ise dosya olduğunu belirtir.** <br/>
İzinlerin harf karşılığı : <br/>
r - : okuma yetkisi (read) <br/>
w - yazma yetkisi (write) <br/>
x - çalıştırma yetkisi (execute) <br/>

**Örneğin; Aşağıdaki dosya izinlerini inceleyelim : ** <br/>
-rw-r--r-- <br/>
**En baştaki - işaretinden dolayı dosya olduğu anlaşılır** <br/>

**Daha sonra diğer ifadeler üçerli parçalara ayrılır.** <br/>
rw- r— r— <br/>
i <br/>
rw- : **dosya sahibinin okuma ve yazma izni olduğunu,** <br/>
r — : **dosya sahibiyle aynı grubun sadece okuma izni olduğunu** <br/>
r — : **diğer tüm kullanıcılar sadece okuma izni olduğunu ifade eder.** <br/>

**Dosya ve dizinlere izin verme** <br/>
**Dosya ve dizinlere izin vermek için chmod komutu çeşitli şekilde kullanılablir.** <br/>
chmod u/g/o/a +/=/- r/w/x <br/>

u : **dosya sahibi (user)** <br/>
g - **dosya sahibibin grubu (group)** <br/>
o - **diğer kullanıcıları (others)** <br/>
a - **tüm hakları (a)** <br/>

(+) - **yetki ekleme** <br/>
= - **yetki eşitleme** <br/>
— : **yetki çıkarma** <br/>
r - **okuma yetkisi (read)** <br/>
w : **yazma yetkisi (write)** <br/>
x - **çalıştırma yetkisi (execute)** <br/>

chmod o+r dosya : **Diğer kullanıcılara yazma izni verir** <br/>
chmod o=r dosya : **ya da bu** <br/>
chmod ugo+rw dosya : **Dosya sahibine dosya sahibinin grubuna ve diğer kullanıcılara yazma ve okuma izni verir.** <br/>
chmod +rw dosya : **Herhangi bir kullanıcı bölümü belirtilmediğinde ifade tüm bölüm için çalışır.** <br/>
stat -c "%a %n" * : **Diğer bir kullanımda stat komutunun çıktısında olduğu gibi sayıların kullanılmasıdır.** <br/>
  
  
**Komut çıktısındaki sayısal ifadeler aşağıdaki şekilde olur.** <br/>

4 - **okuma (read)** <br/>
2 - **yazma (write)** <br/>
1 - **çalıştırma (execute)** <br/>
0 - **yetki alma** <br/>
**Birden fazla izin verileceği zaman verilecek izinler toplanır.** <br/>

**iki rakam dosyanın sahibinin izinlerini, ikinci rakam dosyanın sahibiyle aynı grupta bulunan kullanıcıların yetkilerini, üçüncü rakam diğer kullanıcıların yetkilerini ifade eder.** <br/>

chmod 644 <dosya> <br/>
Dosya sahibi 4 + 2 = 6 okuma ve yazma iznine sahiptir. <br/>
Dosya sahibiyle aynı grup 4 = 4 sadece okuma iznine sahiptir. <br/>
Diğer kullanıcılar 4 = 4 sadece okuma iznine sahiptir. <br/>

chmod 755 <dosya> <br/>
Dosya sahibi 4 + 2 + 1 = 7 okuma, yazma ve çalıştırma iznine sahiptir. <br/>
Dosya sahibiyle aynı grup 4 + 1 = 5 okuma ve yazma iznine sahiptir. <br/>
Diğer kullanıcılar 4 + 1 = 5 okuma ve yazma iznine sahiptir. <br/>

**Dosya ve dizin sahibini değiştirmek <br/>
Dosya sahibini değiştirmek için chown komutu kullanılır.** <br/>
chown <kullanici> <dosya_dizin> <br/>
  
**Değişikliği tüm dizin ve dosyalarda yapmak için R parametresi kullanılır.** <br/>
chown -R <kullanici> <dosya_dizin> <br/>

**Komut linux tabanlı sunucu sistemlerinde sıklıkla kullanılır. <br/>
Dosya sahibini ve grubunu değiştirmek için kullanıcı: grup biçiminde kullanılır.** <br/>
chown -R <kullanici>:<grup> <dosya_dizin> <br/>

**Dosya ve dizin grubunu değiştirmek** <br/>
Dosya grubunu değiştirmek için chgrp komutu kullanılır. <br/>
chgrp <grup> <dosya_dizin> <br/>

**Disk İşlemleri** <br/>
**Linux tabanlı işletim sitemlerinden disk boyutunu öğrenme, bölümleme, biçimlendir, mount etme vb. disk işlemleri ile ilgili disk komutları yer alıyor.** <br/>
Linıx’ta her şey bir dosya olduğundan disk işlemleri diğer işletim sistemlerine göre farlılık gösteriyor. <br/>

**Disk boyutunu öğrenme** <br/>
df : Linux tabanlı işleteim sistemlerinde disk boyutunu öğrenmek için df komutu kullanılır. <br/>
df -h : çıktının daha okunabilir olması için h parametresi kullanılır. <br/>

**Benzer şekilde disk ile ilgili bilgi almak iiçn fdisk, parted, lsblk vb. komut ve araçlarda kullanılabilir.** <br/>
fdisk -l <br/>
parted -l <br/>
lsblk <br/>

**Disk Eşleme <br/>
Linux’da USB takıldığında USB görmüyor gibi sorularla sıklıkla karşılaşılır. Bunun için disk eşleme veya mount etme işleminin yapılması gerekir. <br/>
Disk eşleme öncesi fdisk -l veya lsblk ile eşleme yapılacak diskin yolu bulunur. ** <br/>

mkdir /media/bellek : **Disk yolu bulunduktan sonra media veya mnt dizini içine bir dizin oluşturularak disk eşleme işlemi başlatılır.** <br/>

**Disk eşleme için media ve mnt dizininin kullanımı ve dizin oluşturma zorunlu değildir.** <br/>
mount /dev/sdb1 /media/bellek : **Ancak genellikle media ve mnt dizinleri kullanılır.** <br/>

df -h : **Bağlanan disk boyutunu öğrenmek için de df komutu kullanabiliriz.** <br/>
umount /dev/sdb1 : **Disk eşlemeyi sonlandırmak için umount komutu kullanılır.** <br/>
veya <br/>
umount /media/bellek <br/>

**Disk Bölümleme ve Biçimlendirme** <br/>
fdisk -l : **Sistemdeki diskleri listelemek için I parametresi kullanılır.** <br/>
**Komut çıktı olarak diskleri ve disklerin bölümleriyle ilgili bilgi verir.** <br/>
**Biçimlendirme ve bölümleme işlemi için komuta parametre olarak işlem yapılacak diskin yolu verilir.** <br/>
fdisk /dev/sdb <br/>

**Disk biçimlendirildikten sonra uygun dosya sistemi mkfs komutu ile belirlenerek işlem tamamlanır.** <br/>
mkfs -t <dosya_sistemi> </dev/disk_adi> <br/>
mkfs -t ext4 /dev/sdb1 <br/>

**Disk işlemleri için fdisk komutu kullanılabileceği gibi daha kolay arayüzü olan cfdisk komutu da kullanılabilir.** <br/>
cfdisk /dev/sdb <br/>






