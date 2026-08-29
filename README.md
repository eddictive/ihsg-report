<div align="center">

# 🏛️ TradingSquad AI — IHSG Equity Intelligence Reports
### *Autonomous Multi-Agent AI Research & Market Scanner for Indonesia Stock Exchange (IDX)*

[![IDX Market Intelligence](https://img.shields.io/badge/Market-IDX%20%2F%20IHSG-blue.svg?style=for-the-badge)](https://www.idx.co.id/)
[![AI Architecture](https://img.shields.io/badge/AI%20Engine-TradingSquad%20Orchestrator-8A2BE2.svg?style=for-the-badge)](https://github.com/eddictive)
[![Daily Reports](https://img.shields.io/badge/Reports-Date--Partitioned-green.svg?style=for-the-badge)](#-direktori-laporan)
[![Disclaimer](https://img.shields.io/badge/Compliance-DYOR%20%2F%20No%20Financial%20Advice-red.svg?style=for-the-badge)](#-disclaimer--manajemen-risiko)

<p align="center">
  <b>TradingSquad AI</b> adalah ekosistem analisis pasar modal otonom berbasis <i>Multi-Agent Intelligence Architecture</i> yang dirancang untuk menyajikan riset ekuitas berstandar <i>Institutional-Grade</i> dan pemindaian pasar real-time di Bursa Efek Indonesia (BEI / IDX).
</p>

---

</div>

## 📌 Ikhtisar Repository

Repository ini berfungsi sebagai **arsip publik otomatis** yang memuat seluruh laporan intelijen pasar harian, radar pemindai (*market scanner*), serta analisis komprehensif saham-saham pilihan IDX yang dihasilkan secara langsung oleh orkestrasi agent AI **TradingSquad AI**.

Setiap laporan disusun berdasarkan metodologi keputusan bertingkat (*confluence matrix*) tanpa bias emosional, menggabungkan data aliran bandar (*Bandarmologi*), dinamika mikrostruktur order book, valuasi fundamental kuantitatif, sentimen insider, serta geometri struktur teknikal multi-timeframe.

---

## 🧠 4 Pilar Analisis 360° TradingSquad AI

TradingSquad AI mengorkestrasi 4 mesin (*engines*) spesialis independen untuk menghasilkan **Master Quant Score (0–100)**:

```
                      ┌─────────────────────────────────────────┐
                      │    TRADINGSQUAD AI MASTER ORCHESTRATOR  │
                      └────────────────────┬────────────────────┘
                                           │
         ┌──────────────────┬──────────────┴─────┬──────────────────┐
         ▼                  ▼                    ▼                  ▼
┌─────────────────┐┌─────────────────┐┌──────────────────┐┌──────────────────┐
│  BANDARMOLOGI   ││    TEKNIKAL     ││   FUNDAMENTAL    ││  SENTIMEN/KATALIS│
│ & SMART MONEY   ││    MOMENTUM     ││    KUANTITATIF   ││   & INSIDER FLOW │
│  (Bobot: 40%)   ││  (Bobot: 10-20%)││  (Bobot: 25-35%) ││  (Bobot: 15-20%) │
└────────┬────────┘└────────┬────────┘└─────────┬────────┘└─────────┬────────┘
         │                  │                   │                   │
         └──────────────────┴─────────┬─────────┴───────────────────┘
                                      ▼
                      ┌─────────────────────────────────┐
                      │    MASTER QUANT SCORE (0-100)   │
                      │  Verdicts: ALLOW / REDUCE / BLOCK│
                      └─────────────────────────────────┘
```

### 1. 🐋 Bandarmologi & Smart Money Flow (Institutional Analyst)
* **Broker Accumulation / Distribution:** Pelacakan konsentrasi top buyer/seller institusi lokal, BUMN, dan asing.
* **Smart Money Average Cost:** Mengidentifikasi estimasi harga modal rata-rata bandar pengendali untuk menghitung potensi *asymmetric upside/downside*.
* **Tape Reading & Microstructure (RTVB/HAKA):** Deteksi agresivitas pembelian spontan (*HAKA bursts*), peredaman *shakeout*, hingga identifikasi *spoofing* pada antrean order book.

### 2. 📈 Multi-Timeframe Technical Structure (Technical Analyst)
* **Smart Money Concepts (SMC):** Pemetaan *Fair Value Gaps (FVG)*, *Order Blocks (DBR/RBD)*, dan *Liquidity Sweeps*.
* **Trend & Momentum Stack:** Verifikasi kekuatan tren melalui *Golden Stack MAs*, ADX Trend Intensity, MACD Momentum, dan Chaikin Money Flow (CMF).
* **Orderable Tick-Aligned Geometry:** Penentuan level presisi *Entry, Hard Stop Loss, dan Target Take Profit (TP1/TP2/TP3)* sesuai regulasi fraksi harga resmi IDX.

### 3. 📑 Fundamental Reality & Solvency (Fundamental Analyst)
* **Kualitas Pertumbuhan:** Evaluasi lonjakan pendapatan (*Revenue YoY*) dan pembalikan laba bersih (*Turnaround Net Income*).
* **Solvabilitas & Ketahanan Neraca:** Pengujian model kebangkrutan **Altman Z-Score** dan kekuatan fundamental **Piotroski F-Score**.
* **Valuasi & Margin of Safety:** Estimasi nilai wajar (*Fair Value*) berbasis PE Band Historis, Graham Number, dan rasio utang modal (*DER*).

### 4. 📰 Sentimen, Katalis Makro & Insider Tracking (Sentiment Analyst)
* **Aktivitas Transaksi Insider:** Pelacakan real-time aksi beli/jual pemegang saham pengendali (*KSEI Insider News*).
* **Filings & Aksi Korporasi Resmi:** Sintesis laporan keterbukaan informasi emiten, dividen, ekspansi aset, hingga agenda RUPS / *Public Expose*.
* **Filter Kebisingan Pasar (Anti-Trap):** Memisahkan katalis fundamental riil dari jebakan rumor ritel (*Retail FOMO / Media Hype*).

---

## 🗂️ Direktori & Struktur Laporan

Seluruh laporan diarsipkan secara kronologis berbasis partisi tanggal `YYYY/MM/DD`:

```text
report/
└── YYYY/
    └── MM/
        └── DD/
            ├── [TICKER]_institutional_analysis.md
            ├── [TICKER]_technical_analysis_[mode].md
            ├── [TICKER]_fundamental_analysis.md
            ├── [TICKER]_sentiment_analysis.md
            ├── [TICKER]_detector.md
            └── MARKET_scanner_[focus].md
```

### Konvensi Penamaan Laporan:
| Tipe Laporan | Format Penamaan | Deskripsi |
| :--- | :--- | :--- |
| **Institutional 360°** | `[TICKER]_institutional_analysis.md` | Laporan komprehensif 4 pilar + Master Quant Score |
| **Technical Snapshot** | `[TICKER]_technical_analysis_[mode].md` | Bedah teknikal multi-timeframe (`scalping`, `intraday`, `short_swing`, `swing`, `longterm`) |
| **Sentiment Deep Dive** | `[TICKER]_sentiment_analysis.md` | Analisis sentimen, insider flow & bedah katalis sektoral |
| **Market Scanner Radar**| `MARKET_scanner_[fokus].md` | Radar likuiditas bursa, saham syariah, dan penggerak indeks |

---

## 🎯 Mode Trading & Horizon Analisis

TradingSquad AI mengadaptasi metodologi dan pembobotan skor sesuai horizon waktu transaksi:

| Runtime Mode | Horizon Investasi | Fokus Utama Mesin |
| :--- | :--- | :--- |
| **Scalping** | Intraday / Hit & Run (Detik–Menit) | Live Tape Reading, Microstructure HAKA, Order Book Depth |
| **Intraday** | 1 Sesi – 1 Hari | Intraday VWAP, Momentum Squeeze, Breakout Volatilitas |
| **Short Swing**| 2 – 7 Hari | Fast 4H SMC Structure, Flipped Demand Zones, ADX Momentum |
| **Swing** | 1 – 12 Minggu | Daily Golden Stack, Broker Flow MTF, Turnaround Laba |
| **Long-Term** | 2 – 12 Bulan+ | Fundamental Valuasi, Solvabilitas Neraca, Dividen & Aset |

---

## ⚠️ Disclaimer & Manajemen Risiko

> ### 🛑 PENTING: BUKAN SARAN FINANSIAL ATAU AJAKAN INVESTASI
> 1. Seluruh materi, analisis, tabel skor, dan proyeksi harga yang terdapat dalam repository ini dihasilkan secara otomatis oleh algoritma **TradingSquad AI** untuk tujuan **riset, edukasi, dan studi pasar modal**.
> 2. Laporan ini **BUKAN** merupakan rekomendasi resmi, nasihat investasi, atau ajakan untuk membeli atau menjual efek tertentu dari penasihat keuangan berlisensi.
> 3. Pasar saham memiliki risiko fluktuasi modal dan ketidakpastian. Selalu terapkan prinsip **DYOR (*Do Your Own Research*)**, gunakan manajemen ukuran posisi (*position sizing*) yang bijak, dan pasang batasan risiko (*stop loss*) secara ketat sebelum mengambil keputusan transaksi.
> 4. Pengembang dan kontributor tidak bertanggung jawab atas potensi keuntungan maupun kerugian finansial yang timbul akibat keputusan transaksi yang diambil berdasarkan data dalam repository ini.

---

<div align="center">
  <sub>Developed & Powered by <b>TradingSquad AI</b> · Copyright &copy; 2026 MasEDI.Net</sub>
</div>
