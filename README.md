# Real-Time Syntax Highlighter 
## 🎯 Projeye Erişim<br>
Preojeye github pages aracılığıyla erişilebilir.<br>
https://yagmurerasln.github.io/Real-Time-Syntax-Highlighter/<br><br>

## 📌 Proje Hakkında
Bu proje, hiçbir harici kütüphane kullanmadan geliştirilmiştir. Gerçek zamanlı sözdizimi vurgulayıcı (syntax highlighter) içeren bir grafiksel kullanıcı arayüzü (GUI) uygulamasıdır. Sözdizimsel analiz, biçimsel bir gramer temel alınarak gerçekleştirilmiş olup, analiz süreci iki aşamadan oluşmaktadır:<br>

- **Lexical Analysis** – Giriş kodunun belirli kurallara göre tokenlara ayrılması <br> 
- **Sözdizimsel analiz (Parsing)** – Token akışının context-free grammar (CFG) ile parse edilmesi<br><br>

Uygulama, kullanıcı yazarken anında sözdizimi vurgulaması yapar, 7 farklı token türünü ayırt eder ve parse tree (sentaks ağacı) görselleştirmesini sağlar.<br><br>

## ✨ Özellikler
🍄 Gerçek zamanlı sözdizimi vurgulama<br>
🍄 Token listesi ve türlerine göre istatistik gösterimi  <br>
🍄 Parse tree görselleştirmesi <br> 
🍄 7 token türü (keyword, identifier, string, number, comment, operator, punctuation) <br>
🍄 Klavye kısayolları (örneğin: `Ctrl+S` ile dışa aktarım, `Ctrl+K` ile temizleme)  <br><br>

## 🎨Token Listesi
**KEYWORD:** RENK: #61c863<br>
**IDENTIFIER:** RENK: #f5950e<br>
**STRING:** RENK: #fe79b7<<br>
**NUMBER:** RENK: #8145f8 <br>
**COMMENT:** RENK: #3c7626<br>
**OPERATOR:** RENK: #fbff23<br>
**PUNCTUATION:** RENK: #afb5ff<br><br>

## 🧠 Kullanılan Yöntemler
### 🔤 Lexical Analysis
- **Yöntem:** Durum Diyagramı + Programlama ile gerçekleştirilmiş analiz<br>
- **Amaç:** Kod içerisindeki anahtar kelimeler, tanımlayıcılar, sayılar, string ifadeler, operatörler, yorumlar vb. ayrıştırılır<br>
- **Teknik:** Regular expression'lar yerine doğrudan JavaScript ile yazılmış state-based lexer<br><br>

### 🌳 Sözdizimsel Analiz (Parser)
- **Yöntem:** Top-Down Parser
- **Açıklama:** Preorder gezinti ile parse tree oluşturulmaktadır<br>
- **Gramer:** Proje için tanımlanmış JavaScript benzeri basitleştirilmiş bir context-free grammar (CFG)<br><br>

## 🖥️ Arayüz (GUI)
- Tamamen **HTML, CSS ve Vanilla JavaScript** kullanılarak geliştirilmiştir.<br><br>
- Gerçek zamanlı olarak:<br>
  - Kod yazarken sözdizimi vurgusu<br>
  - Satır numaraları<br>
  - Token istatistikleri (sayılar, anahtar kelimeler vb.)<br>
  - Parse tree (ağaç) yapısının gösterimi<br>
- Dışa aktarma (`.json`) ve düzenleme kolaylığı<br><br>


## 📹 Video ve Makale
[🎞Demo Videosu](https://www.youtube.com/watch?v=zaXuLADMxJI)<br>
[📝Medium Makalesi](https://medium.com/@yagmureraslan55/real-time-syntax-highlighter-ger%C3%A7ek-zamanl%C4%B1-s%C3%B6zdizimi-analizi-ve-parse-tree-g%C3%B6rselle%C5%9Ftirmesi-28eda220f2e1)

