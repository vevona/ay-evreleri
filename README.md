# Ay'ın Evreleri ve Güneş Sistemi · Moon Phases & Solar System

**[Türkçe](#türkçe)** · **[English](#english)**

![Ay'ın evreleri / Moon phases](docs/ay-evreleri.jpg)

**Canlı / Live:** https://vevona.github.io/ay-evreleri/ · https://demo.vevona.com/ay-evreleri/

---

## Türkçe

5\. sınıf Fen Bilimleri "Güneş, Dünya ve Ay" ünitesi için hazırlanmış, tarayıcıda çalışan 3B ders aracı.
Three.js ile yapıldı; kurulum gerektirmez, tek bir HTML dosyası ve dokulardan oluşur.

### Neler var?

**Ay'ın Evreleri**
- Dünya Güneş'in, Ay da Dünya'nın etrafında dolanır; Dünya kendi etrafında döner. Hepsi tek bir zaman saatine bağlıdır, oranlar gerçektir.
- 8 evre (Yeni Ay, Hilal, İlk Dördün, Şişkin Ay, Dolunay, Şişkin Ay, Son Dördün, Hilal) çocuk diliyle açıklanır.
- "Dünya'dan bakınca" penceresi Ay'ın o anki görünüşünü gösterir (Kuzey Yarım Küre).
- Güneş'in aydınlattığı yarı ile Dünya'dan görülen yarının sınırları, Güneş ışınları ve evre adları açılıp kapatılabilir.

**Güneş Sistemi**
- 8 gezegen, Asteroit Kuşağı ve 21 büyük uydu.
- Bir gezegen seçince kamera ona uçar; uyduları yörüngeleriyle görünür. Uyduya tıklayınca yakından izlenir.
- Her gezegen ve uydu için bilgi kartı: uzaklık, çap, gün ve yıl uzunluğu, sıcaklık, uydu sayısı, "Biliyor musun?".
- Satürn'ün halkaları, Uranüs'ün yan yatmış ekseni, Triton'un ters yönde dolanması gibi gerçek ayrıntılar.

![Satürn ve uyduları](docs/saturn.jpg)

### Kullanım

| Tuş | Ay'ın Evreleri | Güneş Sistemi |
| --- | --- | --- |
| `←` `→` | Evreler arasında gez | Gezegenler arasında gez |
| `Boşluk` | Zamanı akıt / durdur | Zamanı durdur / akıt |
| `↑` `↓` | Zamanın hızı | Zamanın hızı |
| `Esc` | | Bir üst görünüme dön |

Fareyle sürükleyerek döndürün, tekerlekle yaklaşın. Sağdaki dikey çubuk zamanın hızını ayarlar
("1 sn = 14 saat" gibi); çift tıklayınca varsayılan hıza döner.

`#gunes-sistemi` adresi uygulamayı doğrudan Güneş Sistemi bölümüyle açar.

### Kendi bilgisayarında ya da sitende çalıştırma

Dosyalar doğrudan bir web sunucusundan yayınlanabilir. Yerelde denemek için:

```bash
python3 -m http.server 8000
```

Ardından http://localhost:8000 adresini açın. (Dokular `file://` ile açıldığında tarayıcı tarafından engellenebilir.)

Kendi sitenize koymak için `index.html` ile `textures/` klasörünü aynı klasöre yüklemeniz yeterli.
Three.js ve yazı tipleri CDN'den yüklenir, bu yüzden internet bağlantısı gerekir.

### Katkı

Hata bildirimi, öneri ve geliştirmeler için issue ya da pull request açabilirsiniz.
Metinler 5. sınıf öğrencilerine göre sade tutulmuştur; bilimsel bir yanlış görürseniz lütfen bildirin.

### Lisans

- **Kod:** [MIT](LICENSE) — dilediğiniz gibi kullanabilir, değiştirebilir ve dağıtabilirsiniz.
- **Dokular:** [Solar System Scope](https://www.solarsystemscope.com/textures/), [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
  Dağıtırken kaynak gösterilmelidir. Ayrıntı: [textures/README.md](textures/README.md).
  Bazı uydu yüzeyleri (İo, Europa, Titan, Triton, İapetus) ve arka plandaki bulutsu kodla üretilir.

---

## English

A browser-based 3D lesson built for the 5th-grade science unit "The Sun, the Earth and the Moon"
(Turkish curriculum). Made with Three.js; no installation or build step — a single HTML file plus textures.
**The interface and all lesson texts are in Turkish.**

### Features

**Moon Phases** (*Ay'ın Evreleri*)
- The Earth orbits the Sun, the Moon orbits the Earth and the Earth spins on its axis. Everything runs on one shared clock, with real ratios.
- All 8 phases (New Moon, Waxing Crescent, First Quarter, Waxing Gibbous, Full Moon, Waning Gibbous, Last Quarter, Waning Crescent) are explained in plain, child-friendly language.
- An "as seen from Earth" window shows how the Moon looks at that moment (Northern Hemisphere).
- Overlays you can toggle: the boundary of the half lit by the Sun, the boundary of the half visible from Earth, sunlight rays and phase labels.

**Solar System** (*Güneş Sistemi*)
- All 8 planets, the Asteroid Belt and 21 major moons.
- Pick a planet and the camera flies to it, showing its moons and their orbits. Click a moon to follow it up close.
- An info card for every planet and moon: distance, diameter, length of day and year, temperature, number of moons, and a "Did you know?" fact.
- Real details such as Saturn's rings, Uranus's sideways tilt and Triton's retrograde orbit.

![Saturn and its moons](docs/saturn.jpg)

### Controls

| Key | Moon Phases | Solar System |
| --- | --- | --- |
| `←` `→` | Previous / next phase | Previous / next planet |
| `Space` | Start / stop time | Stop / start time |
| `↑` `↓` | Time speed | Time speed |
| `Esc` | | Back to the wider view |

Drag to rotate, scroll to zoom. The vertical slider on the right sets how fast time flows
(e.g. "1 sec = 14 hours"); double-click it to reset to the default.

Add `#gunes-sistemi` to the URL to open the app directly in the Solar System section.

### Running it locally or on your own site

The files can be served by any static web server. To try it locally:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000. (Browsers may block the textures when the page is opened via `file://`.)

To host it on your own site, upload `index.html` and the `textures/` folder side by side.
Three.js and the fonts load from a CDN, so an internet connection is required.

### Contributing

Issues and pull requests for bugs, suggestions and improvements are welcome.
The texts are deliberately simple for 10–11-year-olds; if you spot a scientific error, please report it.
Translations of the interface into other languages would also be very welcome.

### License

- **Code:** [MIT](LICENSE) — free to use, modify and redistribute.
- **Textures:** [Solar System Scope](https://www.solarsystemscope.com/textures/), [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
  Attribution is required when redistributing. Details: [textures/README.md](textures/README.md).
  Some moon surfaces (Io, Europa, Titan, Triton, Iapetus) and the background nebula are generated in code.
