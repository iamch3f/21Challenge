# Chat Conversation

Note: _This is purely the output of the chat conversation and does not contain any raw data, codebase snippets, etc. used to generate the output._

### User Input

bu reponun github sayfasında use this template yapıp oraya mı commitlemem gerkiyor şuan

### Planner Response

Merhaba! Sorunuzu daha iyi anlayabilmem için önce mevcut repo yapısına bir bakayım.

*Listed directory [21Challenge](file:///home/chef/Masa%C3%BCst%C3%BC/21Challenge) *

### Planner Response

Bu bir **21 Günlük Challenge** template repo'su gibi görünüyor! Sorunuzu cevaplayayım:

## "Use this template" Kullanımı

**Evet, doğru anlamışsınız!** GitHub'daki template repository'lerde şu şekilde çalışır:

1. **"Use this template"** butonuna tıklarsınız
2. GitHub sizin için **yeni bir repository** oluşturur (orijinal repo'nun bir kopyası olarak)
3. Bu yeni repo **sizin hesabınızda** oluşur
4. Artık bu yeni repo'ya kendi çalışmalarınızı commit'leyebilirsiniz

## Şu an ne yapmalısınız?

Şu an lokal'de `21Challenge` klasörünüzde çalışıyorsunuz. Birkaç seçeneğiniz var:

### Seçenek 1: GitHub'da Template Kullanarak
1. GitHub'daki orijinal repo'da "Use this template" tıklayın
2. Kendi repo'nuzu oluşturun (örn: `benim-21-challenge`)
3. Lokal'deki değişikliklerinizi bu yeni repo'ya push edin

### Seçenek 2: Mevcut Lokal Repo'yu Kullanarak
Eğer zaten bu klasörü clone'ladıysanız:
1. Kendi GitHub'ınızda boş bir repo oluşturun
2. Remote'u değiştirin: `git remote set-url origin <yeni-repo-url>`
3. Değişikliklerinizi push edin

---

**Hangi yöntemi tercih edersiniz?** Eğer henüz başlamadıysanız, **Seçenek 1 (Use this template)** en temiz yoldur çünkü commit geçmişi sıfırdan başlar ve tamamen sizin olur.

### User Input

open in a codespace desem nolur ve reponun içinde use this template yaparken create new repo dedikten sonra isim olarak şunu şunu yap gibi bir yönerge var mı ayrıca haydi 0. ve 1. günü yapalım

### Planner Response

Önce README'yi ve ilk günlerin içeriğini kontrol edeyim, sonra sorularınızı cevaplayıp birlikte başlayalım!

*Viewed [README.md](file:///home/chef/Masa%C3%BCst%C3%BC/21Challenge/README.md) *

*Listed directory [day_00_setup](file:///home/chef/Masa%C3%BCst%C3%BC/21Challenge/day_00_setup) *

*Listed directory [day_01](file:///home/chef/Masa%C3%BCst%C3%BC/21Challenge/day_01) *

### Planner Response

Şimdi Day 0 ve Day 1'in içeriklerini kontrol edeyim:

*Viewed [README.md](file:///home/chef/Masa%C3%BCst%C3%BC/21Challenge/day_00_setup/README.md) *

*Viewed [README.md](file:///home/chef/Masa%C3%BCst%C3%BC/21Challenge/day_01/README.md) *

### Planner Response

Şimdi Day 1'in `main.move` dosyasını kontrol edelim:

*Viewed [main.move](file:///home/chef/Masa%C3%BCst%C3%BC/21Challenge/day_01/sources/main.move) *

### Planner Response

Mükemmel! Şimdi tüm sorularını cevaplayıp başlayalım:

---

## 🔍 Sorularının Cevapları

### 1. "Open in a Codespace" desem ne olur?
**GitHub Codespaces** = Bulutta çalışan bir VS Code ortamı. Tıklarsan:
- GitHub sana bir **sanal makine** açar
- Tarayıcıda VS Code benzeri bir editör açılır
- Sui CLI gibi araçları **kendin kurman** gerekir
- **Dezavantaj**: Her ay ücretsiz 120 saat sınırı var

**Önerim**: Zaten lokal ortamda çalışıyorsun, Codespace'e gerek yok.

### 2. İsimlendirme Yönergesi Var mı?
README'de özel bir isimlendirme yönergesi **yok**, ama mantıklı olanlar:
- `21-day-sui-move` 
- `sui-move-challenge`
- `my-sui-learning`

---

## 🚀 Haydi Başlayalım - Day 0 & Day 1

### Day 0: Setup Kontrolü

Önce Sui CLI'nin kurulu olup olmadığını kontrol edelim:

*User accepted the command `sui --version`*

### Planner Response

Harika! Sui CLI kurulu (`1.62.0`). Şimdi Day 1'in [main.move](cci:7://file:///home/chef/Masa%C3%BCst%C3%BC/21Challenge/day_01/sources/main.move:0:0-0:0) dosyasını tamamlayalım:

*Edited relevant file*

*Edited relevant file*

### User Input

görevleri ben yapacağım oğlumm sen bana mentör ol ve codespaceyi de bir arkadaşıım için sordum bilgisayarı yok ama ipadi var ben use this template yapıp kendi pcmden görevleri yaptıkça gün gün commit etmem mi lazım

### Planner Response

Haha tamam, anladım! 😄 Mentör moduna geçiyorum, kodları sen yazacaksın!

---

## 🎓 Mentör Modunda Cevaplarım

### 1. iPad'den Codespace Kullanımı (Arkadaşın İçin)
**Evet, çalışır!** iPad'de Safari'den GitHub Codespaces açabilir. Ama:
- Sui CLI'yi terminalden kurmak gerekiyor (`suiup install sui@testnet`)
- Dokunmatik klavyeyle kod yazmak zor olabilir
- 120 saat/ay ücretsiz limit var

**Alternatif**: Arkadaşın sadece `move-book.com`'dan okuyup teori öğrenebilir, sonra bilgisayara geçince pratiğe başlar.

---

### 2. Senin İçin Doğru Workflow ✅

**Evet, tam olarak öyle!**

```
1. GitHub'da "Use this template" → "Create a new repository"
2. İsim ver (örn: "sui-21-challenge")
3. Clone'la: git clone https://github.com/SENIN-USERNAME/sui-21-challenge
4. Her gün:
   - Görevi yap
   - Test et: sui move build && sui move test
   - Commit et: git add . && git commit -m "Day X completed"
   - Push et: git push
```

Bu şekilde:
- ✅ GitHub profilinde yeşil kutucuklar (contribution) görünür
- ✅ İlerleme kaydedilir
- ✅ Portföyüne eklenir

---

## 📚 Day 1 Mentörlük

Dosyan açık, TODO kısmını görüyorsun. Görevin:

**Üç tane constant tanımla:**
1. `u64` tipinde bir sayı (örn: yaşın, favori sayın)
2. `bool` tipinde bir değer (true/false)
3. `address` tipinde bir adres (`@0x...` formatında)

**İpucu**: README'deki örneği incele, ama **kendi değerlerini kullan**! Mesela:
```move
const MY_AGE: u64 = 25;
const IS_LEARNING: bool = true;
const WALLET: address = @0xCAFE;
```

Yazdıktan sonra terminalde:
```bash
cd day_01
sui move build
```

**Hata alırsan** bana göster, birlikte çözeriz! 🚀