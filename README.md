AquaGuard AI 🛰️💧

AquaGuard AI, kuraklığa karşı parsel bazlı erken uyarı, 7–14 gün stres tahmini ve akıllı sulama önerisi sunan yapay zeka destekli bir tarım teknolojisi (AgTech) çözümüdür.

Özellikle Konya Havzası gibi yeraltı suyu seviyesinin yıllık 4-5 metre düştüğü ve obruk oluşum riskinin arttığı bölgelerde, su kaynaklarını optimize etmek ve çiftçiyi korumak amacıyla geliştirilmiştir.

📊 Teknik Başarı ve Metrikler

Model Performansı: XGBoost Regressor algoritması ile MAE (Mean Absolute Error) = 0.0619 başarısı sağlandı. Tahminlerimiz %94 oranında yüksek doğruluk içermektedir.

Veri Kaynakları:

Sentinel-2 (Copernicus): NDVI (Bitki Sağlığı) indeksi takibi.

ERA5 (ECMWF): Yağış, sıcaklık ve evapotranspirasyon (buharlaşma) verileri.

Tahmin Penceresi: 7-14 günlük ileriye dönük yüksek doğruluklu stres projeksiyonu.

💡 Temel Özellikler

Erken Uyarı: NDVI anomalilerini anlık iklim sinyalleriyle birleştirerek parsel bazlı stres tespiti yapar.

Yapay Zeka Risk Skoru: 0-100 arası risk puanlaması ile tarlanın gelecekteki sağlık durumunu öngörür.

Akıllı Sulama Önerisi: "Ne zaman ve ne kadar?" sorularına mm cinsinden açıklanabilir (XAI) yanıtlar sunar.

📁 Proje Yapısı

data/: Sentinel-2 & ERA5 veri çekme ve işleme boru hattı (Python).

ml/: XGBoost eğitim scriptleri ve eğitilmiş .pkl modeli.

backend/: FastAPI tabanlı tahmin motoru ve API katmanı.

frontend/: Çiftçiler ve kooperatifler için interaktif dashboard paneli.

🛠️ Kurulum

cd backend && pip install -r requirements.txt

python main.py

Bu proje [Hackathon Adı] kapsamında "AquaGuard AI Team" tarafından geliştirilmiştir.
