<h1 align="center">FIVEM Premium Moderasyon botu UCRETSIZ!</h1>

<p align="center">
  <b>FIVEM Sunucularınızı 10 adım ileriye taşıyacak yenilikçi sistemler, tüm sistemler özenle ve PREMIUM olarak tasarlanmıştır.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/Discord.js_v14-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord.js v14" />
  <img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Komut_Sayısı-49+-blue?style=flat-square" alt="Komut Sayısı" />
  <img src="https://img.shields.io/badge/Event_Handler-21-green?style=flat-square" alt="Event Handler" />
  <img src="https://img.shields.io/badge/Custom_Emoji-34-orange?style=flat-square" alt="Custom Emoji" />
  <img src="https://img.shields.io/badge/Lisans-Proprietary-red?style=flat-square" alt="Lisans" />
</p>

<br>

---

## 📌 Fivem Moderasyon Botu Nedir?

**Paranoid**, Discord sunucuları için sıfırdan tasarlanmış bir yönetim botudur. Ticket sistemi, ekip yönetimi, cezalandırma altyapısı, davet takibi, hoşgeldin kartları, mesaj filtreleme, rol koruma ve çok daha fazlasını tek bir çatı altında sunar.

Her modül bağımsız çalışır, her komut slash command olarak kayıtlıdır ve tüm ayarlar **Redis önbellek** katmanı üzerinden yönetilir. Veritabanı olarak **MongoDB** kullanılır.

> **Developed by Paranoid** — `cinayetlerim` (Discord ID: `323805972101464065`)

<br>

---

## 🎯 Öne Çıkan Özellikler

<br>

### 🎫 Destek & Ticket Sistemi

<p align="center">
  <img src="https://media.discordapp.net/attachments/1090713272031912047/1477292939133583532/image.png?ex=69a43bc3&is=69a2ea43&hm=43a6a7a0dd2e541f0515e36b984a3fd0579c84984e77c8e7975f1545e395c1fb&=&format=webp&quality=lossless&width=568&height=746" alt="Ticket UI" width="480" />
</p>

Paranoid'in destek sistemi, ticket oluşturmadan kapatmaya kadar her adımı otomatikleştirir:

- **7 farklı ticket kategorisi** — IC Sorun, OOC Teknik Sorun, Anticheat, Donate, Diğer, Legal Ekip Başvurusu, Illegal Ekip Başvurusu
- **Ticket Menü** komutu ile kategorileri butonlarla yapılandırılmış embed olarak kanalınıza yerleştirir
- **Sahiplenme sistemi** — Bir yetkili ticket'ı sahiplenir, diğerleri bilgilendirilir
- **Erteleme ve yeniden açma** — Ticket ertelenebilir, kapatılmış ticket geri açılabilir
- **Ticket Top** — En çok ticket kapatan yetkililerin sıralamasını gösterir
- **Kişi ekleme/çıkarma** — Ticket kanalına kullanıcı ekleyip çıkarma
- **Kanal isim değiştirme** — Ticket kanallarının adını anında güncelleme
- **Destek temizleme** — Eski destek verilerini topluca temizleme
- **Sesli destek** — Ticket'a bağlı geçici ses kanalı oluşturma
- **Otomatik log** — Her ticket açılış, kapanış ve sahiplenme işlemi log kanalına kaydedilir

<br>

### 👥 Ekip Yönetim Sistemi

<p align="center">
  <img src="https://media.discordapp.net/attachments/1090713272031912047/1477293093836427334/image.png?ex=69a43be8&is=69a2ea68&hm=3e21a639708f08dec8a9ebc140eedb10033a7e08796a046d17244ab4c17040de&=&format=webp&quality=lossless&width=489&height=545" alt="Ekip Başvuru UI" width="420" />
</p>

Ekip sistemi, sunucunuzdaki tüm ekipleri merkezi olarak yönetir:

| Komut | Açıklama |
|-------|----------|
| `/ekip-oluştur` | Yeni ekip oluşturur (rol, kanal, kategori otomatik) |
| `/ekip-ekle` | Ekibe üye ekler |
| `/ekip-çıkar` | Ekipten üye çıkarır |
| `/ekip-boss` | Ekip liderini değiştirir |
| `/ekip-bilgi` | Ekip detaylarını ve üye listesini gösterir |
| `/ekip-kapat` | Ekibi tamamen kapatır (roller ve kanallar temizlenir) |
| `/ekip-blacklist` | Kullanıcıyı ekip sisteminden kara listeye alır |
| `/ekip-yasakla` | Kullanıcıyı belirli bir ekipten yasaklar |
| `/ekip-senkronize` | Ekip rol/kanal verilerini veritabanıyla senkronize eder |

**Ekip Başvuru Sistemi:**
- Legal ve Illegal olmak üzere **2 ayrı başvuru kategorisi**
- Buton tabanlı başvuru açma
- Otomatik kanal oluşturma ve yetkilendirme
- Başvuru ID'leri ile takip (`LE-0001`, `IE-0001`)

<br>

### ⚖️ Cezalandırma Sistemi

Tam kapsamlı moderasyon altyapısı:

| Komut | Açıklama |
|-------|----------|
| `/ban` | Kullanıcıyı sunucudan yasaklar |
| `/forceban` | Sunucuda olmayan kullanıcıyı yasaklar (tekrar girişte otomatik re-ban) |
| `/uyarı` | Kullanıcıya uyarı verir |
| `/blacklist` | Kullanıcıyı kara listeye alır |
| `/whitelist-ceza` | Whitelist cezası verir |
| `/cezabilgi` | Kullanıcının tüm ceza geçmişini görüntüler |

**Ceza Kaldırma Komutları:**

| Komut | Açıklama |
|-------|----------|
| `/unban` | Yasaklamayı kaldırır |
| `/unforceban` | Forceban cezasını kaldırır |
| `/uyarı-kaldır` | Uyarıyı kaldırır |
| `/blacklist-kaldır` | Kara listeden çıkarır |
| `/whitelistceza-kaldır` | Whitelist cezasını kaldırır |

- 🔁 **Forceban Koruma** — Forceban'lı kullanıcı sunucuya girmeye çalıştığında otomatik olarak tekrar yasaklanır
- 📊 **Ceza Takip** — Tüm ceza işlemleri özel log kanalına detaylı şekilde kaydedilir
- 🆔 Her cezaya benzersiz **Ceza ID** atanır

<br>

### 🎙️ Mülakat Sistemi

- Kullanıcı mülakat bekleme ses kanalına girdiğinde **otomatik özel oda** oluşturulur
- Mülakat tamamlandığında oda otomatik silinir
- Tüm süreç log kanalına kaydedilir

<br>

### 📨 Başvuru & Kayıt

| Komut | Açıklama |
|-------|----------|
| `/whitelist-ver` | Kullanıcıya whitelist rolü verir |
| `/kayıtsız-yap` | Kullanıcının rollerini alır, kayıtsız olarak işaretler |

<br>

### 🛡️ Koruma & Güvenlik Sistemleri

- **Rol Koruma (RoleGuard)** — "Verilemez" olarak işaretlenen rollerin yetkisiz kişiler tarafından verilmesi anında engellenir ve geri alınır
- **Mesaj Filtresi** — Küfür, reklam, spam ve davet linki algılama ve otomatik silme
  - 1000+ kelimelik küfür veritabanı
  - Discord/TikTok/Instagram/Twitter link algılama
  - Spam algılama (tekrar eden mesajlar)
  - Strike sistemi — tekrarlayan ihlallerde otomatik kademeli ceza
- **Forceban Koruma** — Yasaklı kullanıcının sunucuya tekrar girmesini engeller
- **Blacklist Otomatik Rol** — Kara listedeki kullanıcı sunucuya katıldığında otomatik blacklist rolü verilir

<br>

### 🔧 Yönetim Araçları

**Rol Yönetimi:**
| Komut | Açıklama |
|-------|----------|
| `/rol-ver` | Kullanıcıya rol verir |
| `/rol-al` | Kullanıcıdan rol alır |
| `/rol-bilgi` | Rol hakkında detaylı bilgi gösterir |
| `/rol-log` | Rolün son değişiklik geçmişini gösterir |
| `/rolu-aktar` | Bir kullanıcının rollerini başka birine aktarır |
| `/toplu-rolver` | Birden fazla kullanıcıya aynı anda rol verir |
| `/toplu-rolal` | Birden fazla kullanıcıdan aynı anda rol alır |

**Ses Kanalı Yönetimi:**
| Komut | Açıklama |
|-------|----------|
| `/dağıt` | Ses kanalındaki kullanıcıları farklı kanallara dağıtır |
| `/toplu-taşı` | Ses kanalındaki tüm kullanıcıları başka kanala taşır |
| `/toplu-bağlantıkes` | Ses kanalındaki tüm kullanıcıların bağlantısını keser |

**Sunucu Yönetimi:**
| Komut | Açıklama |
|-------|----------|
| `/kilit` | Kanalı kilitler/kilidini açar |
| `/nuke` | Kanalı sıfırlar (aynı ayarlarla yeniden oluşturur) |
| `/sil` | Belirtilen miktarda mesajı siler |

<br>

### 📊 Loglama & İzleme

Paranoid, sunucunuzdaki **her önemli olayı** otomatik olarak loglar:

- 👤 Üye giriş/çıkış logları
- 🔇 Ses kanalı hareketleri (giriş, çıkış, değiştirme, susturma, sağırlaştırma, kamera, yayın)
- 🗑️ Mesaj silme ve düzenleme logları
- 🔨 Ban / Unban logları
- 🎫 Ticket işlem logları
- ⚖️ Ceza işlem logları
- 🛡️ Rol değişiklik logları
- 📨 Davet kullanım logları
- 🤖 Komut kullanım logları (audit trail)

Log kanalları kurulum sırasında otomatik oluşturulur ve kategorilere ayrılır:

```
</> Paranoid Audit
   ├── ◽┃paranoid-giriş
   ├── ◽┃paranoid-çıkış
   ├── ◽┃paranoid-ses
   ├── ◽┃paranoid-yayın
   ├── ◽┃paranoid-kamera
   ├── ◽┃paranoid-mesaj
   ├── ◽┃paranoid-ban
   ├── ◽┃paranoid-rol
   └── ◽┃paranoid-davet

</> Paranoid Sistem
   ├── ◽┃paranoid-komut
   └── ◽┃paranoid-kayıt

</> Paranoid Ticket
   ├── ◽┃paranoid-geçmiş
   └── ◽┃paranoid-yetkili
```

<br>

### 🎨 Hoşgeldin Sistemi

- Sunucuya katılan her üyeye **Canvas ile oluşturulmuş özel hoşgeldin kartı** DM olarak gönderilir
- Kart, kullanıcının avatarı, ismi ve hoşgeldin mesajı içerir
- Otomatik **kayıtsız rolü** atanır
- Hesap yaşı kontrolü — 7 günden yeni hesaplar **"Bot/Spam Şüphesi"** olarak işaretlenir

<br>

### 📩 Davet Takip Sistemi

- Her üyenin **kim tarafından davet edildiği** otomatik tespit edilir
- Davet eden kişinin istatistikleri güncellenir: `Normal`, `Çıkış`, `Sahte`
- 7 günden yeni hesaplar **sahte davet** olarak sayılır
- Üye çıkışında davet edenin istatistikleri güncellenir

<br>

### 📝 IC İsim Senkronizasyonu

- Özel bir kanala yazılan isimler doğrulanır (regex ile format kontrolü)
- Yetkili onayı ile kullanıcının Discord ismi güncellenir
- Red/Onay butonları ve sebep belirtme sistemi

<br>

### ⚙️ Kurulum Sihirbazı

`/kurulum` komutu ile sunucu tamamen otomatik yapılandırılır:

1. **Rol Kayıt** — Tüm sistem rollerini (kayıtsız, whitelist, blacklist, yetkili rolleri vb.) seçmeniz için interaktif menü
2. **Kanal Kayıt** — Mülakat bekleme, IC isim kanalı gibi özel kanalları eşleştirme
3. **Log Kanal Kurulumu** — Tüm log kategorileri ve kanalları otomatik oluşturulur
4. **Tam Kurulum** — Hepsini tek seferde sıralı olarak yapar

Ek olarak:
- `/ayarlar` — Tüm bot ayarlarını detaylı olarak görüntüler ve değiştirir
- `/kurulum-bilgi` — Mevcut kurulum durumunu özetler
- `/database-sıfırla` — Tüm bot verilerini sıfırlar (kanallar, roller, DB kayıtları)

<br>

---

## 🎭 34 Adet Özel Emoji

Paranoid, **34 adet custom emoji** kullanarak tüm mesajlarına profesyonel bir görünüm kazandırır. Bu emojiler botun Discord uygulama emojileri olarak tanımlanır ve tüm sunucularda çalışır.

Emoji listesi: `paranoidicon`, `pAktif`, `pBakim`, `pBaglanti`, `pCezalandirma`, `pCheater`, `pFiree`, `pFolder`, `pInfo`, `pIslemBilgi`, `pIslemYapan`, `pIslemYapilan`, `pKalp`, `pLoading`, `pLog`, `pNo`, `pPartner`, `pPasif`, `pSettings`, `pStaff`, `pTarih`, `pTicket`, `pWarning`, `pYes`, `pYildiz`, `pYukleniyor`, `pMember` ve emoji sayaçlar (`psifir` — `pdokuz`).

> 🎨 **Emojileri almak için** Discord üzerinden iletişime geçin: `cinayetlerim` (`323805972101464065`)

<br>

---

## ⚡ Mimari & Teknoloji

```
Paranoid/
├── Core/
│   ├── paranoindex.js          ← Ana giriş noktası & bootstrap
│   ├── Database/               ← MongoDB şemaları (6 model)
│   │   ├── Ceza.js             ← Ceza kayıtları
│   │   ├── Ekip.js             ← Ekip verileri
│   │   ├── Invites.js          ← Davet takibi
│   │   ├── Tickets.js          ← Ticket kayıtları
│   │   ├── User.js             ← Kullanıcı verileri
│   │   └── YetkiliPuan.js      ← Yetkili performans puanları
│   └── Settings/               ← JSON config dosyaları
│       ├── SunucuAyarlar.json
│       ├── SunucuKanallar.json
│       ├── SunucuLogKanallar.json
│       ├── SunucuRoller.json
│       └── BadWords.json       ← Küfür veritabanı
├── Commands/                   ← Slash command modülleri (49 dosya)
│   ├── Başvuru/                ← Ekip başvuru menüsü
│   ├── Cezalandırma/           ← Ban, uyarı, blacklist + geri alma
│   ├── Destek/                 ← Ticket komutları (8 komut)
│   ├── Ekip/                   ← Ekip yönetim komutları (9 komut)
│   ├── Mülakat/                ← Mülakat sistemi
│   ├── Root/                   ← Kurulum ve yönetici araçları
│   └── Yonetim/                ← Rol, ses ve sunucu yönetimi
│       ├── Rol/                ← 7 rol komutu
│       ├── Ses/                ← 3 ses komutu
│       └── Sunucu/             ← 3 sunucu komutu
├── Events/                     ← Event handler modülleri (21 dosya)
│   ├── TicketEvents.js
│   ├── EkipEvents.js
│   ├── EkipBasvuruEvents.js
│   ├── MulakatEvents.js
│   ├── MessageFilter.js
│   ├── RoleGuard.js
│   ├── ICIsimEvents.js
│   ├── Hosgeldin.js
│   └── ...
├── Helpers/                    ← Yardımcı modüller (10 dosya)
│   ├── RedisConfigManager.js   ← Redis önbellek yönetimi
│   ├── AuthChecker.js          ← Yetki kontrol sistemi
│   ├── ContainerBuilder.js     ← Discord Components V2 builder
│   ├── GetEmoji.js             ← Custom emoji sistemi
│   ├── LogSender.js            ← Merkezi loglama
│   ├── EmbedBuilder.js
│   ├── EkipUI.js
│   └── ...
├── LICENSE
├── package.json
└── README.md
```

### Redis Önbellek Katmanı

Tüm ayar dosyaları uygulama başlangıcında Redis'e yüklenir. Her okuma işlemi önce Redis'ten karşılanır, Redis'te yoksa diskten okunur ve cache'e yazılır (**hydrate-on-miss**). Yazma işlemlerinde hem disk hem Redis eş zamanlı güncellenir. Redis bağlantısı koparsa sistem otomatik olarak **dosya fallback** moduna geçer.

### Discord Components V2

Paranoid, Discord'un yeni **Components V2** (`ContainerBuilder`) API'sini kullanır. Tüm bot mesajları `ParanoidContainer` sınıfı üzerinden oluşturulur ve her mesajın altına otomatik olarak `Paranoid Bot's` footer'ı eklenir.

<br>

---

## 🛠️ Kurulum

### 1. Gereksinimler

| Yazılım | Versiyon | Açıklama |
|---------|----------|----------|
| **Node.js** | v18+ | [nodejs.org](https://nodejs.org/) |
| **MongoDB** | — | Ücretsiz [MongoDB Atlas](https://www.mongodb.com/atlas) hesabı yeterli |
| **Redis** | v5+ | Aşağıdaki adımla kolayca kurulur |

### 2. Redis Kurulumu (Windows)

Redis, veritabanı sorgularını hızlandıran bir önbellek katmanıdır. Windows'ta kurmak çok basittir:

1. **[Redis for Windows](https://github.com/tporadowski/redis/releases/tag/v5.0.14.1)** sayfasına gidin
2. `Redis-x64-5.0.14.1.msi` dosyasını indirin
3. Normal bir program gibi "İleri (Next)" diyerek kurulumu tamamlayın
4. Kurulumdan sonra Redis arka planda otomatik çalışmaya başlar

> 💡 Linux/macOS kullanıyorsanız: `sudo apt install redis-server` veya `brew install redis`

### 3. Projeyi Hazırlama

```bash
# 1. Repoyu klonlayın
git clone https://github.com/KULLANICI_ADINIZ/Paranoid.git
cd Paranoid

# 2. Bağımlılıkları yükleyin
npm install
```

### 4. Ortam Değişkenlerini Ayarlama

`Core/Settings/` dizinindeki `.env` dosyasını düzenleyin:

```env
TOKEN=DISCORD_BOT_TOKENINIZ
GUILD_ID=SUNUCU_ID
MONGO_URI=mongodb+srv://KULLANICI:SIFRE@cluster.mongodb.net/paranoid
REDIS_URL=redis://127.0.0.1:6379
```

> ⚠️ **Token ve veritabanı bilgilerinizi asla paylaşmayın!**

### 5. Botu Başlatma

```bash
npm start
```

Bot başlatıldığında:
1. MongoDB bağlantısı kurulur
2. Redis bağlantısı kurulur ve ayarlar önbelleğe alınır
3. 49+ slash komut Discord'a kaydedilir
4. 21 event handler yüklenir
5. 34 custom emoji yüklenir

İlk kurulumda sunucunuzda `/kurulum` komutunu kullanarak açılan panelden roller, kanallar ve log kanallarını yapılandırın.

<br>

### 🚀 7/24 Kesintisiz Çalıştırma (PM2)

VDS veya sunucu üzerinde çalıştırıyorsanız:

```bash
# PM2'yi global olarak yükleyin
npm install -g pm2

# Botu PM2 ile başlatın
pm2 start Core/paranoindex.js --name "paranoid"

# Sunucu yeniden başlatmalarında otomatik çalışması için
pm2 save
pm2 startup
```

<br>

---

## 🎯 Servis & İletişim

Bu botu kendi sunucunuz için **servis olarak kurdurmak** istiyorsanız veya **özel emojileri** almak istiyorsanız Discord üzerinden iletişime geçebilirsiniz:

<p align="center">
  <a href="https://discord.com/users/323805972101464065">
    <img src="https://img.shields.io/badge/Discord-cinayetlerim-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" />
  </a>
</p>

<br>

---

## 🖼️ Görseller
<p align="center">
  <img src="https://media.discordapp.net/attachments/1090713272031912047/1477296749373558865/Ekran_goruntusu_2026-02-27_225359.png?ex=69a43f4f&is=69a2edcf&hm=e1b7b151c8b2876d075c3e5c720b505bb9a5d41d8b2bea85e20feb0f31d698ac&=&format=webp&quality=lossless&width=346&height=247" alt="Görsel 1" width="600" />
</p>

<p align="center">
  <img src="https://media.discordapp.net/attachments/1090713272031912047/1477296885831176263/Ekran_goruntusu_2026-02-27_235933.png?ex=69a43f70&is=69a2edf0&hm=84aec3b0a5d9da01aa03a98ef014b7581db569f8e9804f2cc2083f719a0ea272&=&format=webp&quality=lossless&width=515&height=769" alt="Görsel 2" width="600" />
</p>

<br>

---

## ⚖️ Lisans

Bu proje **Paranoid Proprietary License** altında lisanslanmıştır.

```
Copyright (c) 2024-2026 cinayetlerim (Discord ID: 323805972101464065)
Tüm hakları saklıdır.
```

- ✅ Kişisel ve ticari olmayan kullanım **serbesttir**
- ❌ Kopyalama, dağıtım ve ticari satış **yasaktır**
- ❌ İçerisindeki isimlerin değiştirilmesi **yasaktır**
- ❌ İzinsiz türev çalışmalar **yasaktır**

Detaylar için [LICENSE](./LICENSE) dosyasına bakın.

<br>

---

<p align="center">
  <img src="https://img.shields.io/badge/Developed_by-Paranoid-000000?style=for-the-badge" alt="Developed by Paranoid" />
</p>

<p align="center">
  <sub>Discord FIVEM sunucu yönetiminde yeni standart. ⚡</sub>
</p>
