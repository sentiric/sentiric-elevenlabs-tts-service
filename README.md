# ✨ Sentiric ElevenLabs TTS Service (Expert TTS Engine)

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![Python Version](https://img.shields.io/badge/python-3.11+-blue.svg)](https://www.python.org/)

**Sentiric ElevenLabs TTS Service**, `sentiric-tts-gateway-service` tarafından yönetilen **uzman ses motorlarından** biridir. Temel amacı, ElevenLabs'in premium API'sini kullanarak **markaya özel, ultra-realistik ve duygusal** sesler üretmektir.

Bu servis, en yüksek kalitede ses deneyimi gerektiren kurumsal müşteriler ve özel projeler için kullanılır.

## 🎯 Temel Sorumluluklar

*   **Premium Sentezleme:** ElevenLabs API'sine istek atarak, metni sese dönüştürür.
*   **Özel Ses Desteği:** Müşterilerin kendi ElevenLabs hesaplarında tanımladıkları özel ses ID'lerini (`voice_id`) kullanmalarını sağlar.
*   **API Adaptörü:** `tts-gateway`'den gelen standart sentezleme isteğini, ElevenLabs API'sinin beklediği formata çevirir.

## 🛠️ Teknoloji Yığını

*   **Dil:** Python
*   **Web Çerçevesi:** FastAPI (planlanan)
*   **API İstemcisi:** `httpx`

## 🔌 API Etkileşimleri

*   **Gelen (Sunucu):**
    *   `sentiric-tts-gateway-service` (REST/JSON veya gRPC): Ses sentezleme isteklerini alır.
*   **Giden (İstemci):**
    *   `api.elevenlabs.io`: Sentezleme işlemini gerçekleştirmek için.

## 🚀 Yerel Geliştirme

1.  **Bağımlılıkları Yükleyin:** `pip install -r requirements.txt`
2.  **`.env` Dosyasını Oluşturun:** `ELEVENLABS_API_KEY`'inizi girin.
3.  **Servisi Başlatın:** `uvicorn app.main:app --reload`

## 🤝 Katkıda Bulunma

Katkılarınızı bekliyoruz! Lütfen projenin ana [Sentiric Governance](https://github.com/sentiric/sentiric-governance) reposundaki kodlama standartlarına ve katkıda bulunma rehberine göz atın.

---
## 🏛️ Anayasal Konum

Bu servis, [Sentiric Anayasası'nın (v11.0)](https://github.com/sentiric/sentiric-governance/blob/main/docs/blueprint/Architecture-Overview.md) **Zeka & Orkestrasyon Katmanı**'nda yer alan merkezi bir bileşendir.