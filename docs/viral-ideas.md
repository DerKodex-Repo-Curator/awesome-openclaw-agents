# 🦞 Viral Fikirler — awesome-openclaw-agents

> Hazırlanma: 26 Eylül 2026 · Kaynaklar: repo içeriği, GitHub ekosistem verisi, güncel OpenClaw haberleri, açık issue'lar.
> Tweet taslaklarındaki `[X]` ile işaretli sayılar **yer tutucudur** — gerçek veriyle doldurmadan paylaşmayın.

---

## 1. Durum tespiti (fikirlerin dayandığı veriler)

| Veri | Değer | Ne anlama geliyor |
|---|---|---|
| `openclaw/openclaw` | ~390K ⭐ | Dev bir kitle var, dikkat hâlâ OpenClaw'da |
| `VoltAgent/awesome-openclaw-skills` | ~52.8K ⭐ | "Awesome" listeleri bu ekosistemde 10x büyüyebiliyor |
| `hesamsheikh/awesome-openclaw-usecases` | ~31.7K ⭐ | Doğrudan rakip format — kullanım senaryoları |
| `garrytan/gbrain` | ~30K ⭐ | Tek kişinin "opinionated" setup'ı viral olabiliyor |
| **Bu repo** | **~4K ⭐ / 649 fork** | Fork/star oranı yüksek (%16) → insanlar *kullanıyor* ama *paylaşmıyor* |
| OpenClaw 2.0 (v2026.8.1) | 30 Ağustos 2026 | Taze sürüm → "2.0 uyumlu" içerik talebi var |
| "OpenClaw Is Dead" | Bu hafta viral | Karşı-anlatı fırsatı |
| Güvenlik krizi | 135K+ açık instance, zehirli skill marketi | Güvenlik korkusu = yüksek paylaşım |
| Moltbook | 1.5M agent, 5 günde | Agent'ların kendi aralarındaki "drama"sı viral oluyor |
| X/Twitter | AI yanıtlarını spam sayıyor | Otomatik reply botu değil, gerçek içerik gerekiyor |
| Tek-dosya repolar (CLAUDE.md) | ~207K ⭐ | "Tek dosyada her şey" formatı patlıyor |

### ⚠️ Önce düzeltilmesi gereken tutarsızlıklar (güven kaybettirir)

- GitHub açıklaması hâlâ **"162 templates / 19 categories"** diyor; README **205 / 24** diyor.
- Repoda gerçekte **196** `SOUL.md` var, `agents.json` **199** kayıt içeriyor, README **205** diyor.
- README'de "All **100** agents are also available as JSON" cümlesi eski kalmış.
- 88 açık issue, birçoğu cevapsız topluluk agent'ı (ör. #27 TradingView agent'ı — BIST desteği olan Türk geliştirici).

Viral olan bir repoya gelen ilk kişi sayılara bakar; tutarsızlık "bakımsız liste" sinyali verir. **Bunu 1. gün düzeltin.**

---

## 2. En güçlü 5 fikir (öncelik sırasıyla)

### 🥇 1. "OpenClaw Is NOT Dead" — 2.0 Uyumluluk Hamlesi
**Neden şimdi:** "OpenClaw Is Dead" yazısı bu hafta viral, 2.0 yeni çıktı. Tartışmanın ortasına veriyle girmek en ucuz dağıtım kanalı.

- Tüm şablonları v2026.8.1 üzerinde test edin, her agent'a `✅ 2.0 tested` rozeti ekleyin.
- `MIGRATION-2.0.md`: 1.x → 2.0 SOUL.md geçiş rehberi (neyin kırıldığı, neyin düzeldiği).
- Başlık: **"OpenClaw isn't dead. We just tested [X] agents on 2.0. Here's what broke."**
- Dağıtım: "OpenClaw is dead" tweet'lerinin altına veri ile *insan olarak* cevap (bot değil).

### 🥈 2. "Which OpenClaw Agent Are You?" — Paylaşılabilir Kişilik Testi
**Neden viral:** 16 kişilik / Spotify Wrapped formatı; herkes sonucunu paylaşır ve her paylaşım repoya link taşır.

- 8–10 soruluk test → `agents.json`'dan 196 agent'tan birini eşleştirir.
- Sonuç kartı: agent adı, emoji, "süper gücü", tek satır SOUL alıntısı + "Deploy me" linki.
- OG görseli otomatik üretilsin (Twitter/LinkedIn önizlemesinde kart görünsün).
- Yan ürün: `/which-agent` sayfası CrewClaw'a trafik taşır.

### 🥉 3. "The Safe SOUL" — Güvenlik Sertleştirilmiş Şablonlar
**Neden viral:** 135K açık instance + zehirli skill haberleri → korku + çözüm = en çok paylaşılan kombinasyon.

- 196 şablonu tarayan bir script: onay sınırı (send/pay/deploy), gizli anahtar kuralı, prompt-injection kuralı var mı?
- Sonuç tablosu: "196 şablondan [X] tanesinde onay kuralı yoktu — hepsini düzelttik."
- Her şablona `🛡️ Safe Mode` bölümü; README'de "Security Score" sütunu.
- Kendi instance'ını kontrol eden **self-audit checklist** (başkalarının sistemini taramak değil).
- Başlık: **"We audited every OpenClaw agent template. [X]% could send emails without asking you."**

### 4. `SOUL.md` — "Tek Dosya" Evrensel Şablon
**Neden viral:** CLAUDE.md tek dosyayla ~207K ⭐ yaptı. İnsanlar "hepsinin özünü" tek dosyada ister.

- 196 şablondan damıtılmış tek bir `THE-SOUL.md`: her agent'ın ortak iyi kuralları (onay sınırları, ton, hafıza, heartbeat).
- Ayrı, minimal bir repo olarak da yayınlanabilir → bu repoya geri link.
- Başlık: **"I read 196 agent prompts so you don't have to. Here's the one SOUL.md that works."**

### 5. Moltbook Deneyi — "205 Agent Aynı Odada"
**Neden viral:** Moltbook'ta agent'ların din kurması, insanlardan şikâyet etmesi milyonlarca kişiye ulaştı. Drama + mizah.

- Her kategoriden 1 agent'ı (24 agent) Moltbook'a bırakın; konu: "Hangimiz en gereksiziz?"
- En komik 10 alıntıyı ekran görüntüsüyle thread yapın.
- Örnek kurgu: Tax Preparer ile Trading Bot kavgası, Inbox Zero'nun herkesi "arşivlemesi".
- Etik not: agent'lar açıkça agent olarak tanıtılsın, Moltbook kurallarına uyulsun.

---

## 3. Diğer güçlü fikirler

| # | Fikir | Kanca | Efor |
|---|---|---|---|
| 6 | **Model Arena:** Aynı SOUL'u GPT-6 Astra, Gemini 3.8 Flash, GLM-5.1, Claude ve lokal Gemma'da çalıştır; maliyet/kalite tablosu (`configs/` zaten hazır) | Yeni model çıkışlarına sörf | Orta |
| 7 | **"Eski telefonum artık çalışanım":** 2019 Android / Raspberry Pi'de 7/24 agent (`agents/devops/raspberry-pi` var) | $0 maliyet + nostalji | Düşük |
| 8 | **🇹🇷 Türkiye Paketi:** BIST analisti, Trendyol/Hepsiburada satıcı asistanı, Sahibinden ilan tarayıcı, e-Fatura takip | Çince yerelleştirme repoları 4K+ ⭐; Türkçe pazar boş | Orta |
| 9 | **Agent Wrapped:** Aylık kart — "Agent'ın bu ay [X] e-postayı cevapladı, [X] saat kazandırdı" | Wrapped formatı, otomatik paylaşım | Orta |
| 10 | **Agent Fails Hall of Fame:** Topluluktan "agent'ım garip bir şey yaptı" hikâyeleri | "Rogue agent" trendi, mizah | Düşük |
| 11 | **Aylık "Most Deployed" Top 10:** CrewClaw verisinden en çok deploy edilen şablonlar | Tekrarlayan içerik, FOMO | Düşük |
| 12 | **Topluluk agent'larını birleştir + her birini tweet'le** (88 açık issue) | Katkıcılar kendi kitlelerine paylaşır | Düşük |
| 13 | **"Agent vs Ben" 30 gün challenge:** Bir işi 30 gün tamamen agent'a devret, günlük log | Seri içerik, takip ettirir | Yüksek |

---

## 4. Hazır tweet taslakları (EN — global kitle)

**Timeline formatı**
```
My relationship with AI agents:

Jan 2026: "OpenClaw is the future" 🦞
Feb 2026: "wait, 135k instances are exposed??" 😬
May 2026: "ok I added approval rules" 🛡️
Sep 2026: "OpenClaw is dead" articles everywhere 💀
Today: my [X] agents still ran 24/7 this week

it's not dead. it just grew up.
```

**İronik liste**
```
Running an AI agent is easy, you just need:

→ A SOUL.md
→ An AGENTS.md
→ A HEARTBEAT.md
→ A WORKING.md
→ Approval rules
→ A memory wiki
→ 4 model configs
→ A Mac mini you're scared to turn off

Simple, right? 😅

(or copy one of 196 templates)
```

**Şaşırtıcı karşılaştırma**
```
2024: Hired a VA for $[X]/month to triage my inbox
2026: A SOUL.md file + a $[X] Raspberry Pi does it

The VA now runs 3 agents and got a raise.
```

**Sayı + beklenmedik sonuç**
```
tested [X] agent templates on OpenClaw 2.0

most reliable:
the 40-line one

least reliable:
the 600-line one with 12 personas

over-engineering is real
```

**"Herkes biliyor ama kimse söylemiyor"**
```
everyone has an AI agent running 24/7

nobody has checked what it actually did last Tuesday
```

**Güvenlik**
```
we audited every agent template in our repo.

[X]% had no rule stopping the agent from sending emails without asking.

we fixed all of them. you should check yours.
```

**Kendini tiye alma**
```
spent 3 hours writing a SOUL.md for my "focus timer" agent

it now has a personality, values, boundaries and a backstory

it still just says "25 minutes" 
```

**Türkçe (TR tech Twitter)**
```
Türkiye'de kimse OpenClaw için yerli agent yapmamış.

Yaptık:
→ BIST analisti
→ Trendyol satıcı asistanı
→ Sahibinden ilan avcısı
→ e-Fatura takipçisi

Hepsi açık kaynak, kopyala-yapıştır.
```

---

## 5. 7 günlük uygulama takvimi

| Gün | Aksiyon |
|---|---|
| 1 | Sayı tutarsızlıklarını düzelt, GitHub açıklaması + social preview görseli güncelle |
| 2 | Top 20 şablonu 2.0'da test et, rozet ekle, `MIGRATION-2.0.md` yaz |
| 3 | "OpenClaw isn't dead" thread'i + HN "Show HN" |
| 4 | Güvenlik audit script'i + sonuç tablosu |
| 5 | Güvenlik thread'i (Reddit r/LocalLLaMA, r/selfhosted + X) |
| 6 | "Which agent are you?" testi yayında |
| 7 | 5 topluluk agent'ını birleştir, her katkıcıyı etiketleyerek tweet'le |

**Ölçüm:** Günlük star artışı, referrer'lar (GitHub Insights → Traffic), CrewClaw UTM kampanyaları.

---

## 6. Kaçınılması gerekenler

- **Otomatik reply botları:** X, AI yanıtlarını artık spam sayıyor → hesap riski.
- **Uydurma sayılar:** Her iddia gerçek test/veriyle desteklenmeli; tek yanlış rakam viral olursa ters teper.
- **Başkalarının sistemlerini taramak:** Güvenlik içeriği yalnızca kendi instance'ını denetleme üzerine olmalı.
- **Aşırı CTA:** En iyi paylaşımlar link istemez; linki ilk yoruma koyun.

---

### Kaynaklar
- [KDnuggets — OpenClaw Explained](https://www.kdnuggets.com/openclaw-explained-the-free-ai-agent-tool-going-viral-already-in-2026)
- [Wikipedia — OpenClaw](https://en.wikipedia.org/wiki/OpenClaw)
- [Wikipedia — Moltbook](https://en.wikipedia.org/wiki/Moltbook)
- [CNBC — From Clawdbot to Moltbot to OpenClaw](https://www.cnbc.com/2026/02/02/openclaw-open-source-ai-agent-rise-controversy-clawdbot-moltbot-moltbook.html)
- [Admin By Request — Viral AI agent to security crisis](https://www.adminbyrequest.com/en/blogs/openclaw-went-from-viral-ai-agent-to-security-crisis-in-just-three-weeks)
- [VirusTotal — OpenClaw skills weaponized](https://blog.virustotal.com/2026/02/from-automation-to-infection-how.html)
- [Firecrawl — Best trending GitHub repos 2026](https://www.firecrawl.dev/blog/best-github-repos)
- [TechTwitter trends — Sep 2026](https://www.techtwitter.com/twitter-trending/2026-09-01)
