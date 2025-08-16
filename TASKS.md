# ✨ Sentiric ElevenLabs TTS Service - Görev Listesi

Bu belge, `elevenlabs-tts-service`'in geliştirme yol haritasını ve önceliklerini tanımlar.

---

### Faz 1: Temel Servis İskeleti (Sıradaki Öncelik)

Bu faz, servisin fonksiyonel bir API adaptörü haline getirilmesini hedefler.

-   [ ] **Görev ID: TTS-EL-001 - FastAPI Sunucusu Kurulumu**
    -   **Açıklama:** `/api/v1/synthesize` ve `/health` endpoint'lerini içeren temel bir FastAPI uygulaması oluştur.
    -   **Durum:** ⬜ Planlandı.

-   [ ] **Görev ID: TTS-EL-002 - ElevenLabs API Entegrasyonu**
    -   **Açıklama:** Gelen isteği ElevenLabs API formatına dönüştüren, isteği gönderen ve dönen ses verisini (MP3/WAV) istemciye geri ileten mantığı implemente et.
    -   **Durum:** ⬜ Planlandı.

-   [ ] **Görev ID: TTS-EL-003 - Dinamik Ses ID'si**
    -   **Açıklama:** API isteğine `voice_id` parametresi ekleyerek, `.env`'deki varsayılan ses yerine isteğe özel bir sesin kullanılmasını sağla.
    -   **Durum:** ⬜ Planlandı.

-   [ ] **Görev ID: TTS-EL-004 - Dockerfile Oluşturma**
    -   **Açıklama:** Servisi konteyner içinde çalıştırabilmek için optimize edilmiş bir `Dockerfile` oluştur.
    -   **Durum:** ⬜ Planlandı.