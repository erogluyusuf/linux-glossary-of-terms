# 1. **Çevresel Değişkenler ve Sistem Bilgisi**
| Komut      | Akılda Kalıcı Bilgi                                           | Açıklama                                                       | Syntax Örneği                               |
|------------|---------------------------------------------------------------|---------------------------------------------------------------|---------------------------------------------|
| `printenv` | "Print" (yazdırmak) ve "env" (çevresel değişkenler) birleşimi  | Çevresel değişkenleri görüntüler.                             | `printenv`                                  |
| `env`      | "Environment" (çevre) kısaltması                              | Çevresel değişkenleri görüntüler, bazen komut çalıştırmak için de kullanılır. | `env`                                      |
| `$PATH`    | "Path" (yol) kelimesi, çalıştırılabilir dosyaların bulunduğu dizinleri ifade eder | Çalıştırılabilir dosyaların bulunduğu dizinleri belirler.     | `echo $PATH`                                |
| `$`        | Değişkenlerin başında yer alır, "dolar işareti" ile değişken gösterimi | Shell içerisinde değişkenleri temsil eder.                   | `echo $HOME`                                |
| `lsb_release` | "Linux Standard Base" (Linux Standart Temeli) ve "release" (sürüm) birleşimi | Linux dağıtım bilgilerini görüntüler.                    | `lsb_release -a`                            |
| `uname`    | "Unix Name" (Unix ismi) kısaltması                           | Sistem hakkında bilgi verir.                                  | `uname -a`                                  |
| `hostname` | "Host" (sunucu) ve "name" (isim) birleşimi                    | Sistemin adını görüntüler.                                    | `hostname`                                  |
| `who`      | "Who" (kim) kelimesi, kimlerin sisteme giriş yaptığını sorgular | Sistemde oturum açmış kullanıcıları gösterir.                 | `who`                                       |
| `uptime`   | "Up" (yukarıda) ve "time" (zaman) birleşimi                  | Sistemin çalışma süresini ve yükünü görüntüler.              | `uptime`                                    |

---

# 2. **Sistem Yönetimi ve Yardım Komutları**
| Komut      | Akılda Kalıcı Bilgi                                           | Açıklama                                                       | Syntax Örneği                               |
|------------|---------------------------------------------------------------|---------------------------------------------------------------|---------------------------------------------|
| `help`     | "Help" (yardım) kelimesi, komut hakkında yardım verir        | Bir komutun kullanım bilgilerini görüntüler.                  | `help <komut_adı>`                          |
| `man`      | "Manual" (kılavuz) kelimesinin kısaltması                      | Komutun detaylı kullanım kılavuzunu gösterir.                 | `man <komut_adı>`                           |
| `whatis`   | "What is" (ne nedir?) sorusunun kısaltması                    | Komut hakkında kısa bir açıklama gösterir.                    | `whatis <komut_adı>`                        |
| `apropos`  | "Apropos" (ilgili) kelimesi, arama ile ilişkili komutları bulur | Aranan kelimeyle ilgili komutları listeler.                   | `apropos <anahtar_kelime>`                  |
| `synopsis`| Komutun genel yapısını tanımlar (genelde man sayfalarında).  | Komutun genel yapısını tanımlar.                              | `man <komut_adı>`                           |
| `description` | "Description" (açıklama) kelimesi, komutun ne yaptığına dair bilgi verir | Komutun ne yaptığına dair detaylı açıklama.              | `man <komut_adı>`                           |
| `example`  | "Example" (örnek) kelimesi, komutun örnek kullanımlarını sunar  | Komutun örnek kullanımı.                                      | `man <komut_adı>`                           |
| `see also` | "See also" (ayrıca bakınız) kelimesi, ilgili komutları belirtir | İlgili komutlar hakkında bilgi verir.                         | `man <komut_adı>`                           |
| `mandb`    | "Manual database" (kılavuz veritabanı) kısaltması              | Man sayfalarını günceller.                                    | `mandb`                                     |

---

# 3. **Dosya ve Dizin Yönetimi**
| Komut      | Akılda Kalıcı Bilgi                                           | Açıklama                                                       | Syntax Örneği                               |
|------------|---------------------------------------------------------------|---------------------------------------------------------------|---------------------------------------------|
| `mkdir`    | "Make directory" (dizin oluşturmak) kelimelerinin birleşimi     | Yeni bir dizin oluşturur.                                      | `mkdir <dizin_adı>`                         |
| `rm`       | "Remove" (silmek) kelimesinin kısaltması                       | Dosya veya dizinleri siler.                                    | `rm <dosya_adı>`                            |
| `tar`      | "Tape archive" (bant arşivi) kelimelerinin birleşimi            | Arşiv dosyaları oluşturur, çıkarır veya içeriğini görüntüler.  | `tar -xvzf <arşiv_dosyası.tar.gz>`         |
| `gzip`     | "GNU zip" (GNU sıkıştırma) kelimelerinin birleşimi              | Dosyaları sıkıştırmak için kullanılır.                         | `gzip <dosya_adı>`                          |
| `bzip2`    | "Burrows-Wheeler" (sıkıştırma algoritması) ve "zip" kelimelerinin birleşimi | Yüksek sıkıştırma oranı ile dosya sıkıştırır.                   | `bzip2 <dosya_adı>`                         |
| `gunzip`   | "GNU unzip" (GNU sıkıştırmayı açmak) kelimelerinin birleşimi    | `.gz` uzantılı dosyaları açar.                                 | `gunzip <dosya_adı.gz>`                     |
| `bunzip2`  | "Burrows-Wheeler unzip" (Burrows-Wheeler sıkıştırmayı açmak)    | `.bz2` uzantılı dosyaları açar.                                | `bunzip2 <dosya_adı.bz2>`                   |
| `zcat`     | "Zipped cat" (sıkıştırılmış dosya içeriğini görüntülemek)      | Sıkıştırılmış dosyaların içeriğini görüntüler.                 | `zcat <dosya_adı.gz>`                       |
| `zgrep`    | "Zipped grep" (sıkıştırılmış dosyalarda arama yapmak)          | Sıkıştırılmış dosyalarda arama yapar.                          | `zgrep <arama_kelimesi> <dosya_adı.gz>`     |
| `bzcat`    | "Bzip2 cat" (Burrows-Wheeler sıkıştırma açmak)                  | `.bz2` dosyasını açar ve içeriğini gösterir.                   | `bzcat <dosya_adı.bz2>`                     |
| `bzgrep`   | "Bzip2 grep" (Burrows-Wheeler sıkıştırmasında arama yapar)      | `.bz2` dosyasında arama yapar.                                 | `bzgrep <arama_kelimesi> <dosya_adı.bz2>`   |
| `unrar`    | "UnRAR" (RAR arşivini açmak) kelimesinin birleşimi              | `.rar` arşiv dosyasını açar.                                   | `unrar x <dosya_adı.rar>`                   |
| `unzip`    | "Unzip" (zip dosyasını açmak) kelimesinin birleşimi             | `.zip` arşiv dosyasını açar.                                   | `unzip <dosya_adı.zip>`                     |

---

# 4. **Kullanıcı ve İzin Yönetimi**
| Komut      | Akılda Kalıcı Bilgi                                           | Açıklama                                                       | Syntax Örneği                               |
|------------|---------------------------------------------------------------|---------------------------------------------------------------|---------------------------------------------|
| `chmod`    | "Change mode" (mod değiştirmek) kelimelerinin birleşimi        | Dosya veya dizinlerin erişim izinlerini değiştirir.            | `chmod 755 <dosya_adı>`                     |
| `chown`    | "Change owner" (sahibi değiştirmek) kelimelerinin birleşimi    | Dosya veya dizinlerin sahibini değiştirir.                     | `chown <kullanıcı_adı>:<grup_adı> <dosya_adı>` |
| `export`   | "Export" (ihracat) kelimesi, çevresel değişkenleri bir alt shell'e aktarır | Değişkenleri bir alt shell'e aktarır.                         | `export <değişken_adı>=<değer>`             |
| `suid` bit | "Set User ID" (Kullanıcı ID'sini ayarla) bit'i                 | Bir dosyanın çalıştırılmasında, dosyanın sahibinin kimliğiyle çalışılmasını sağlar. | `chmod u+s <dosya_adı>`                   |
| `find / -perm -! -type l -ls` | "Find" (bulmak) komutu ve `-perm` (izinler) ve `-type` (tip) seçenekleri | Belirli izinlere sahip olmayan ve link olmayan dosyaları listeler. | `find / -perm -! -type l -ls` |
| `rws`      | "Read Write Set" (Okuma yazma ve set bit'i) anlamına gelir      | Dosya izinlerinde setuid, setgid ve sticky bit’i ifade eder.   | `chmod u+s <dosya_adı>`                     |
| `chattr`   | "Change attribute" (özellik değiştirmek) kısaltması            | Dosya özelliklerini değiştirmeye yarar.                        | `chattr +i <dosya_adı>`                     |
| `lsattr`   | "List attribute" (özellik listelemek) kısaltması               | Dosya özelliklerini listeler.                                  | `lsattr <dosya_adı>`                        |
| `adduser`  | "Add user" (kullanıcı ekle) kelimesinin birleşimi               | Yeni kullanıcı ekler.                                           | `adduser <kullanıcı_adı>`                   |
| `useradd`  | "User add" (kullanıcı eklemek) kelimesinin birleşimi            | Yeni kullanıcı hesabı oluşturur.                                | `useradd <kullanıcı_adı>`                   |
| `userdel`  | "User delete" (kullanıcı sil) kelimesinin birleşimi             | Kullanıcıyı siler.                                              | `userdel <kullanıcı_adı>`                   |
| `vipw`     | "Vi password" (vi ile şifre düzenlemek) kelimelerinin birleşimi | `/etc/passwd` dosyasını düzenler.                               | `vipw`                                      |
| `vigr`     | "Vi group" (vi ile grup düzenlemek) kelimelerinin birleşimi     | `/etc/group` dosyasını düzenler.                                | `vigr`                                      |
| `chage`    | "Change age" (yaş değiştir) kelimelerinin birleşimi             | Kullanıcı şifre değiştirme süresi üzerinde değişiklik yapar.   | `chage -M 90 <kullanıcı_adı>`               |
| `usermod`  | "User modify" (kullanıcıyı değiştirmek) kelimelerinin birleşimi | Kullanıcı hesabını değiştirir.                                  | `usermod -aG <grup_adı> <kullanıcı_adı>`    |
| `passwd`   | "Password" (şifre) kelimesinin birleşimi                        | Kullanıcı şifresini değiştirir.                                 | `passwd <kullanıcı_adı>`                    |

---

# 5. **Sistem Durumu ve İşlem Yönetimi**
| Komut      | Akılda Kalıcı Bilgi                                           | Açıklama                                                       | Syntax Örneği                               |
|------------|---------------------------------------------------------------|---------------------------------------------------------------|---------------------------------------------|
| `w`        | "Who" (kim) kelimesi, hangi kullanıcıların sisteme giriş yaptığını gösterir | Sistemdeki aktif kullanıcıları ve oturum bilgilerini gösterir.  | `w`                                         |
| `who`      | "Who" (kim) kelimesi, kimlerin sisteme giriş yaptığını sorgular | Sistemde oturum açmış kullanıcıları listeler.                   | `who`                                       |
| `whoami`   | "Who am I" (ben kimim) sorusunun kısaltması                    | Şu anda oturum açmış kullanıcının adını gösterir.              | `whoami`                                    |
| `su`       | "Switch user" (kullanıcıyı değiştir) kelimelerinin birleşimi    | Başka bir kullanıcı olarak sisteme giriş yapar.                | `su <kullanıcı_adı>`                        |
| `ps`       | "Process status" (işlem durumu) kelimelerinin birleşimi        | Çalışan işlemleri gösterir.                                    | `ps aux`                                    |
| `top`      | "Table of processes" (işlem tablosu) kelimelerinin birleşimi   | Sistem kaynaklarını kullanan işlemleri gösterir.                | `top`                                       |
| `htop`     | "High-level top" (yüksek seviye top) kelimelerinin birleşimi   | `top` komutunun gelişmiş versiyonudur.                          | `htop`                                      |
| `kill`     | "Kill" (öldürmek) kelimesi, işlemleri sonlandırır             | Bir işlemi sonlandırır.                                        | `kill <işlem_id>`                           |
| `killall`  | "Kill all" (tümünü öldürmek) kelimelerinin birleşimi           | Belirli bir isme sahip tüm işlemleri sonlandırır.               | `killall <işlem_adı>`                       |
| `pkill`    | "Process kill" (işlem öldürmek) kelimelerinin birleşimi        | Belirli bir kritere göre işlemleri sonlandırır.                 | `pkill <işlem_adı>`                         |
# 6. **Ağ Yönetimi ve İnternet Komutları**
| Komut      | Akılda Kalıcı Bilgi                                           | Açıklama                                                       | Syntax Örneği                               |
|------------|---------------------------------------------------------------|---------------------------------------------------------------|---------------------------------------------|
| `ping`     | "Packet Internet Groper" (İnternet Paket Gruplaması) kelimelerinin birleşimi | Ağ bağlantısını test eder.                                    | `ping <ip_adresi>`                          |
| `ifconfig` | "Interface configuration" (Ağ arayüz yapılandırması) kelimelerinin birleşimi | Ağ arayüzlerinin yapılandırmasını görüntüler.                 | `ifconfig`                                  |
| `ip`       | "Internet Protocol" (İnternet Protokolü) kısaltması            | Ağ yapılandırması ve ağ arayüzlerini yönetir.                 | `ip addr show`                              |
| `traceroute`| "Trace route" (yol takibi) kelimelerinin birleşimi             | Ağ üzerindeki paketlerin izlediği yolu gösterir.               | `traceroute <ip_adresi>`                    |
| `nslookup` | "Name Server Lookup" (Ad Sunucu Araması) kısaltması            | DNS sorguları yapar, bir alan adının IP adresini bulur.        | `nslookup <domain_adı>`                     |
| `dig`      | "Domain Information Groper" (Alan Adı Bilgisi Araştırıcısı)    | DNS hakkında detaylı bilgi verir.                             | `dig <domain_adı>`                          |
| `netstat`  | "Network statistics" (Ağ istatistikleri) kısaltması            | Ağ bağlantılarını ve durumunu gösterir.                       | `netstat -tuln`                             |
| `curl`     | "Client URL" (İstemci URL) kısaltması                         | URL üzerinden veri alır veya gönderir.                         | `curl <url_adresi>`                         |
| `wget`     | "World Wide Web Get" (WWW'den veri alma) kısaltması            | Dosya indirmek için kullanılır.                               | `wget <url_adresi>`                         |
| `ssh`      | "Secure Shell" (Güvenli Kabuk) kısaltması                      | Uzaktaki bir makineye güvenli bağlantı kurar.                 | `ssh <kullanıcı_adı>@<ip_adresi>`           |
| `scp`      | "Secure Copy" (Güvenli Kopyalama) kısaltması                   | Dosyaları güvenli bir şekilde uzak bir makineye kopyalar.      | `scp <dosya_adı> <kullanıcı_adı>@<ip_adresi>:<hedef_dizin>` |
| `ftp`      | "File Transfer Protocol" (Dosya Transfer Protokolü) kısaltması | Dosya transferi yapmak için kullanılır.                        | `ftp <ip_adresi>`                           |

---

# 7. **Sistem Bakımı ve İzleme**
| Komut      | Akılda Kalıcı Bilgi                                           | Açıklama                                                       | Syntax Örneği                               |
|------------|---------------------------------------------------------------|---------------------------------------------------------------|---------------------------------------------|
| `df`       | "Disk Free" (Disk Boş) kelimelerinin birleşimi                | Disk kullanımını ve boş alanı görüntüler.                     | `df -h`                                     |
| `du`       | "Disk Usage" (Disk Kullanımı) kelimelerinin birleşimi         | Dosya ve dizinlerin disk kullanımını gösterir.                 | `du -sh <dizin_adı>`                        |
| `free`     | "Free" (boş) kelimesi, sistemin bellek kullanımını gösterir   | Bellek ve swap alanı kullanımını gösterir.                     | `free -h`                                   |
| `uptime`   | "Up" (yukarıda) ve "time" (zaman) birleşimi                  | Sistemin ne kadar süredir çalıştığını gösterir.                | `uptime`                                    |
| `iostat`   | "Input/output statistics" (Giriş/çıkış istatistikleri)        | Disk I/O (giriş/çıkış) istatistiklerini gösterir.              | `iostat`                                    |
| `vmstat`   | "Virtual Memory Statistics" (Sanal Bellek İstatistikleri)     | Sanal bellek ile ilgili istatistikleri gösterir.               | `vmstat`                                    |
| `dmesg`    | "Diagnostic Message" (Tanılama Mesajı) kısaltması             | Çekirdek ve donanım mesajlarını görüntüler.                   | `dmesg`                                     |
| `sysctl`   | "System Control" (Sistem Kontrolü) kısaltması                  | Çekirdek yapılandırmalarını ayarlar ve görüntüler.             | `sysctl -a`                                 |
| `journalctl`| "Journal Control" (Jurnal Kontrolü) kısaltması               | Sistem günlüklerini görüntüler.                               | `journalctl`                                |

---

# 8. **Yedekleme ve Arşivleme**
| Komut      | Akılda Kalıcı Bilgi                                           | Açıklama                                                       | Syntax Örneği                               |
|------------|---------------------------------------------------------------|---------------------------------------------------------------|---------------------------------------------|
| `rsync`    | "Remote Sync" (Uzak Senkronizasyon) kelimelerinin birleşimi    | Dosya ve dizinleri senkronize eder, yedekleme yapar.           | `rsync -avz <kaynak> <hedef>`               |
| `tar`      | "Tape Archive" (Bant Arşivi) kelimelerinin birleşimi           | Dosyaları arşivler ve sıkıştırır.                              | `tar -czvf <arşiv_adı.tar.gz> <dosya_adı>`   |
| `cp`       | "Copy" (kopyalamak) kelimesinin kısaltması                    | Dosya veya dizinleri kopyalar.                                 | `cp <kaynak> <hedef>`                       |
| `mv`       | "Move" (taşımak) kelimesinin kısaltması                       | Dosya veya dizinleri taşır.                                    | `mv <kaynak> <hedef>`                       |
| `dd`       | "Data Description" (Veri Tanımı) kısaltması                   | Düşük seviyeli disk yedekleme ve veri transferi yapar.         | `dd if=<giriş_dosya> of=<çıkış_dosya>`      |
| `cpio`     | "Copy In and Out" (İçeri ve Dışarı Kopyalama) kelimelerinin birleşimi | Dosya arşivleme ve yedekleme komutudur.                     | `cpio -idmv <arşiv_dosyası>`                |

---

# 9. **Disk ve Dosya Sistemi Yönetimi**
| Komut      | Akılda Kalıcı Bilgi                                           | Açıklama                                                       | Syntax Örneği                               |
|------------|---------------------------------------------------------------|---------------------------------------------------------------|---------------------------------------------|
| `fdisk`    | "Fixed Disk" (Sabit Disk) kelimelerinin birleşimi             | Disk bölümleri oluşturur veya düzenler.                        | `fdisk /dev/sda`                            |
| `parted`   | "Partition Editor" (Bölüm Editörü) kısaltması                 | Disk bölümleriyle ilgili işlemler yapar.                       | `parted /dev/sda`                           |
| `mkfs`     | "Make File System" (Dosya Sistemi Oluşturmak) kısaltması       | Dosya sistemi oluşturur.                                       | `mkfs.ext4 /dev/sda1`                       |
| `fsck`     | "File System Check" (Dosya Sistemi Kontrolü) kısaltması        | Dosya sistemini kontrol eder ve onarır.                        | `fsck /dev/sda1`                            |
| `mount`    | "Mount" (Bağlamak) kelimesi, dosya sistemini bağlar            | Dosya sistemini bağlamak için kullanılır.                      | `mount /dev/sda1 /mnt`                      |
| `umount`   | "Unmount" (Çıkarmak) kelimesi, bağlanmış dosya sistemini çıkartır | Bağlı dosya sistemini çıkartır.                               | `umount /mnt`                               |
| `df`       | "Disk Free" (Disk Boş) kelimelerinin birleşimi                | Disk kullanımını ve boş alanı gösterir.                        | `df -h`                                     |
| `du`       | "Disk Usage" (Disk Kullanımı) kelimelerinin birleşimi         | Dosya ve dizinlerin disk kullanımını gösterir.                 | `du -sh <dizin_adı>`                        |
