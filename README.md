# Hasta Sıralama Çözüm Aracı v4 / Patient Scheduling Optimization Tool v4

[![GitHub Pages](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue)](https://kurutkan.github.io/Hasta-s-ralay-c-/)

---

## Türkçe

### Hakkında

Hasta Sıralama Çözüm Aracı, sağlık kuruluşlarında hasta kuyruğu yönetimini optimize eden, tarayıcı tabanlı bir simülasyon aracıdır. Monte Carlo simülasyonu, çok algoritmali sıralama kuralları ve gerçek zamanlı klinik performans analitiği ile çalışır.

### Özellikler

- **6 Sıralama Algoritması:** FCFS (İlk gelen ilk alınır), SPT (En kısa süre önce), LPT (En uzun süre önce), SVF (En küçük varyans önce), NSR (En düşük no-show riski önce), HYB (Ağırlıklı hibrit skor)
- **Monte Carlo Simülasyonu:** Stokastik tekrarlarla maliyet, bekleme süresi ve fazla mesai dağılımları üretir
- **Hizmet Süresi Dağılımları:** Lognormal ve Gamma dağılımları desteklenir
- **Çoklu Sunucu Desteği:** 1–5 paralel hekim ile simülasyon
- **Walk-in Hasta Modeli:** Poisson süreci ile randevusuz hasta girişi
- **Overbooking Analizi:** No-show telafisi için kapasite üstü kabul senaryoları
- **Maliyet Analizi:** Kademeli bekleme, boşta kalma ve fazla mesai maliyet hesaplamaları
- **Senaryo Karşılaştırma:** Farklı hasta sayıları için toplu simülasyon
- **Gantt Diyagramı:** Hasta bazlı görsel zaman çizelgesi
- **Radar Grafiği:** Algoritmaların çok boyutlu performans karşılaştırması

### Kullanım

1. [Canlı demo](https://kurutkan.github.io/Hasta-s-ralay-c-/) bağlantısını açın
2. "Veri girişi" sekmesinde sistem parametrelerini ve hasta bilgilerini düzenleyin
3. "Simüle et" butonuna tıklayarak Monte Carlo simülasyonunu başlatın
4. Diğer sekmelerde (Sıralama, Maliyet, No-show + OB, Performans, Senaryo) sonuçları inceleyin

### Gereksinimler

Herhangi bir kurulum gerektirmez. Modern bir tarayıcı (Chrome, Firefox, Edge, Safari) yeterlidir. Tüm bağımlılıklar CDN üzerinden yüklenir.

---

## English

### About

Patient Scheduling Optimization Tool is a browser-based simulation tool that optimizes patient queue management in healthcare facilities. It leverages Monte Carlo simulation, multi-algorithm scheduling rules, and real-time clinic performance analytics.

### Features

- **6 Scheduling Algorithms:** FCFS (First Come First Served), SPT (Shortest Processing Time), LPT (Longest Processing Time), SVF (Smallest Variance First), NSR (No-Show Risk first), HYB (Weighted hybrid score)
- **Monte Carlo Simulation:** Generates cost, wait time, and overtime distributions via stochastic replications
- **Service Time Distributions:** Supports Lognormal and Gamma distributions
- **Multi-Server Support:** Simulate with 1–5 parallel physicians
- **Walk-in Patient Model:** Unscheduled patient arrivals via Poisson process
- **Overbooking Analysis:** Over-capacity acceptance scenarios to offset no-shows
- **Cost Analysis:** Tiered waiting, idle time, and overtime cost calculations
- **Scenario Comparison:** Batch simulation across different patient volumes
- **Gantt Chart:** Patient-level visual timeline
- **Radar Chart:** Multi-dimensional performance comparison of algorithms

### Usage

1. Open the [live demo](https://kurutkan.github.io/Hasta-s-ralay-c-/)
2. Configure system parameters and patient data in the "Veri girişi" (Data Entry) tab
3. Click "Simüle et" (Simulate) to run the Monte Carlo simulation
4. Explore results across tabs: Sıralama (Scheduling), Maliyet (Cost), No-show + OB, Performans (Performance), Senaryo (Scenario)

### Requirements

No installation required. A modern browser (Chrome, Firefox, Edge, Safari) is sufficient. All dependencies are loaded via CDN.

---

## Tech Stack

- **React 18** — UI components with hooks
- **Recharts** — Data visualization (BarChart, RadarChart, LineChart)
- **Tailwind CSS** — Utility-first styling
- **Babel Standalone** — In-browser JSX transformation
- **Vanilla JavaScript** — Monte Carlo engine, queue processing, statistical sampling

## File Structure

| File | Description |
|------|-------------|
| `index.html` | Standalone HTML application (no build step required) |
| `patient_queue_optimizer_v4.jsx` | Original React/JSX source code |

## License

This project is open source and available for academic and research purposes.
