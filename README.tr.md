<!-- CURRENT-SKILL-PUBLICATION -->
![Evidence Research Skills](assets/collection-hero.svg)

# Evidence Research Skills

11 skill: kaynak araştırma, araç seçimi ve doğrulanabilir sonuç üretme için hazır iş akışları. Modelin ağırlıklarını değiştirmez; sonuç kalitesi kullanılan kaynaklara ve araçlara bağlıdır.

[![Download ChatGPT](https://img.shields.io/badge/ChatGPT-Download_ZIP-10a37f?style=for-the-badge)](https://github.com/yigityildiz0/evidence-research-skills/raw/refs/heads/main/downloads/ChatGPT.zip) [![Download Claude](https://img.shields.io/badge/Claude-Download_ZIP-d97757?style=for-the-badge)](https://github.com/yigityildiz0/evidence-research-skills/raw/refs/heads/main/downloads/Claude.zip)

**ChatGPT:** bütün listelenen skilleri içeren eklenti paketini indir; hesabının desteklediği kişisel eklenti/skill içe aktarma akışını kullan. Tek-skill ChatGPT bağlantısı, tek skill içeren eklenti ZIP’idir. **Claude:** toplu ZIP’i aç, içindeki tekil skill ZIP’lerini ayrı ayrı yükle. Dış ZIP tek bir Claude skill’i değildir. Yerel kurulum bulut hesabına yükleme yapmaz.

Türkçe veya İngilizce doğal isteklerle kullan: “literatür tara / search literature”, “makale değerlendir / appraise paper”, “fizyo vakasını analiz et / assess physio case”. Kısa kelimeler seçim ipuçlarıdır; bütün platformlarda aynı slash menüsünü oluşturmaz. Mevcut iş akışları ve güvenlik kuralları korunmuştur.

## Skill listesi

| Skill | Çözdüğü sorun / örnek istek | ChatGPT | Claude |
|---|---|---|---|
| [`medical-evidence-research`](skills/common/medical-evidence-research/SKILL.md) | Literatür tara; makaleyi değerlendir; güncel kanıtı bul | [↓ ZIP](packages/chatgpt/medical-evidence-research.zip) | [↓ ZIP](packages/claude/medical-evidence-research.zip) |
| [`physio-clinical-copilot`](skills/common/physio-clinical-copilot/SKILL.md) | Fizyo vakasını analiz et; rehabilitasyon planla | [↓ ZIP](packages/chatgpt/physio-clinical-copilot.zip) | [↓ ZIP](packages/claude/physio-clinical-copilot.zip) |
| [`research-analyst`](skills/common/research-analyst/SKILL.md) | Araştır; iddiayı doğrula; karşıt kanıtları incele | [↓ ZIP](packages/chatgpt/research-analyst.zip) | [↓ ZIP](packages/claude/research-analyst.zip) |
| [`primary-source-research`](skills/common/primary-source-research/SKILL.md) | Birincil kaynaklardan doğrula; kaynaklı not hazırla | [↓ ZIP](packages/chatgpt/primary-source-research.zip) | [↓ ZIP](packages/claude/primary-source-research.zip) |
| [`gemini-deep-research`](skills/common/gemini-deep-research/SKILL.md) | Gemini ile kaynaklı derin araştır | [↓ ZIP](packages/chatgpt/gemini-deep-research.zip) | [↓ ZIP](packages/claude/gemini-deep-research.zip) |
| [`parallel-web`](skills/common/parallel-web/SKILL.md) | Çoklu web kaynağını paralel araştır | [↓ ZIP](packages/chatgpt/parallel-web.zip) | [↓ ZIP](packages/claude/parallel-web.zip) |
| [`academic-study-coach`](skills/common/academic-study-coach/SKILL.md) | Bir konuyu öğret; makaleyi açıkla; sınava hazırla | [↓ ZIP](packages/chatgpt/academic-study-coach.zip) | [↓ ZIP](packages/claude/academic-study-coach.zip) |
| [`data-analyst`](skills/common/data-analyst/SKILL.md) | Tabloyu analiz et; istatistikleri açıkla | [↓ ZIP](packages/chatgpt/data-analyst.zip) | [↓ ZIP](packages/claude/data-analyst.zip) |
| [`ai-research-skills`](skills/common/ai-research-skills/SKILL.md) | AI araştırma fikri üret; deney veya makale planla | [↓ ZIP](packages/chatgpt/ai-research-skills.zip) | [↓ ZIP](packages/claude/ai-research-skills.zip) |
| [`graphify`](skills/common/graphify/SKILL.md) | Belgeler veya kod arasında bilgi grafiği çıkar | [↓ ZIP](packages/chatgpt/graphify.zip) | [↓ ZIP](packages/claude/graphify.zip) |
| [`office-docs-qa`](skills/common/office-docs-qa/SKILL.md) | PDF, Word, Excel veya sunumu kontrol et | [↓ ZIP](packages/chatgpt/office-docs-qa.zip) | [↓ ZIP](packages/claude/office-docs-qa.zip) |

## Teknik bilgiler

Claude açıklamaları en fazla 200 karakterdir; her skill paketi en fazla 200 dosya içerir. Kaynaklar, yardımcı betikler ve lisanslar paketlenir. `ai-research-skills` için mevcut bulut alt kümesi ile tam yerel kaynak ayrı tutulur; paketlenmemiş modüller bulut paketinin içinde varmış gibi gösterilmez. API anahtarları, ücretli erişim, yerel CLI ve canlı veri bağlantıları paketin parçası değildir. Kontroller paket yapısını ve kaynak eşleşmesini doğrular; hesapta yükleme, klinik doğruluk veya yatırım performansı testi yapıldığı anlamına gelmez. [Bütünlük değerleri](downloads/SHA256SUMS.txt) · [Kaynak ve lisans bilgisi](THIRD_PARTY_NOTICES.md).

Klinik çıktılarda özet/tam metin, çalışma kalitesi/raporlama, istatistiksel anlamlılık/klinik önem ayrılır. Skill bireysel tanı koymaz ve klinisyenin yerini almaz.


[AI research security repair / Güvenlik düzeltmesi](AI-RESEARCH-SECURITY.md): 98 local / 10 cloud modules retained; explicit scope, privacy and permission boundaries.


## From question to defensible evidence / Sorudan kanıta

1. Define a PICO/PECO or diagnostic/measurement question, population, outcomes and eligibility criteria.
2. Search PubMed/MEDLINE and relevant PEDro, DiTA, Cochrane/CENTRAL and allied-health sources. Combine controlled vocabulary with text synonyms; translate syntax per database. Add Turkish/English TR Dizin, DergiPark and YÖK searches when relevant.
3. Record database, exact query, date, filters and retrieval count; deduplicate and explain screening decisions. Track access limits rather than claiming inaccessible sources were searched.
4. Verify DOI/PMID, publication version, peer review, corrections/retractions and full-text access. Use study-design-appropriate appraisal; separate risk of bias from reporting quality, effect sizes from p-values, and ICC/SEM/MDC/MCID from each other.
5. Compare supporting and conflicting findings, applicability, uncertainty and clinical importance. Do not present an abstract-only read as a full-text appraisal. Reuse a saved query for updates; actual recurring alerts require user scheduling authorization.

See the skill's [source map](skills/common/medical-evidence-research/references/source-map.md) and [search strategy](skills/common/medical-evidence-research/references/search-strategy.md). Youthall and Marmara's supplied pages are discovery guides; DergiPark hosts journals. None replaces study-level appraisal.

Türkçe örnek: “Literatür tara: donuk omuzda egzersiz dozu; arama dizgilerini göster, karşıt çalışmaları da bul ve klinik önemi açıkla.”
English example: “Appraise this rehabilitation paper; verify its version, methods, effect sizes, bias and applicability, and label any unavailable full text.”

<!-- END-CURRENT-SKILL-PUBLICATION -->

