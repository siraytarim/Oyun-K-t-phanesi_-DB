## Proje Adı: Oyun Kütüphanesi
<br>

### Proje Ekibi : Sıray TARIM, Sevgi PEKİN, Ahmet Salih DOĞAN
<br>


### Proje Gereksinimleri:
<br>

- Kullanıcı olabilmek için mail ve şifre gerekir. (1:1)

- Bir kullanıcı bir hesaba giriş yapabilir. (1:1)

- Mail onayından sonra bir kullanıcı için bir id belirlenir. (1:1)

- Platformda birden çok kullanıcı olabilir. (1:N)

- Bir oyuncu birden çok oyuna sahip olabilir. (1:N)

- Bir oyunun birçok kullanıcısı olabilir. (1:N)

- Bir oyunun bir geliştiricisi olabilir. (1:1)

- Bir geliştiricinin birden çok oyunu olabilir. (1:N)

- Bir oyunu yayımlayan bir şirket olabilir. (1:1)

- Bir şirketin yayımladığı birçok oyun olabilir. (1:N)

- Bir kullanıcı bir oyuna geribildirim yapabilir. (1:1)

- Platform içindeki oyunlara kategorilerden ulaşılabilir. (N:M)

- Kategori bölümü bir tane olabilir içerisinde türler bulunur. (1:N)

- Türler kısmının içerisinde oyunların türlerine ait genel başlıklar ve onların alt başlıkları bulunur. (1:N)

- Türler kendi içlerinde birkaç alt başlığa ayrılabilir. (Bknz. Aksiyon – Arcade ve Ritim , Birinci Şahıs Nişancı vb.) (1:N)

- Oyunların sağladığı işletim sistemleri için de macOS, Steam OS + Linux için bulunur. (N:M)

- En çok satanlar kısmının içerisinde türlerine ve tarih bilgisine göre en çok satın alınan oyunlar bulunur. 

- Oyunlar; oyun id, oyun adı, türü, fiyatı, çıkış tarihi, yazılımcısı, yayımcısı, sağlandığı sistemler, geri bildirimi gibi bilgilere sahiptir. 


<br>

### İlişkisel Şema:   
<br>

**Kullanıcılar**
- u_id: int
- u_Name: varchar
- u_date: datetime
- u_SiteLink: varchar
- u_username: varchar
- u_ProfilePic: varchar
- u_about: varchar
- u_Age: int
  
<br>

**Kullanıcı Girişi**
- u_username: varchar
- u_password: varchar

<br>

**Kullanıcı Kaydı**
- u_mail: varchar
- u_password: varchar

<br>

**Oyunlar**
- g_id: int
- g_Name: varchar
- g_ReleaseTime: datetime
- g_Dev: varchar
- g_Pub: varchar
- g_Type: varchar
- g_Price: smallmoney
- g_OS: varchar
- g_review: int

<br>

**Kategoriler**
- ca_id: int
- ca_name: varchar

<br>

**Türler**
- t_id: int
- t_name: varchar

<br>

**Görüşler**
- u_id: int
- r_comment: varchar
- r_votes: int

<br>

**Yayımlayan**
- p_id: int
- p_name: varchar

<br>

**Geliştirici**
- d_id: int
- d_name: varchar

<br>

## E-R Diyagramı :
<br>

![210260060_210260100_210260020_Oyun_Kütüphanesi 2 -page-001](https://github.com/user-attachments/assets/1033a5e8-5c7f-4d66-a9f9-9ac80e248b95)






  


