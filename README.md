# Cinema Club Profile Analyzer

Kadrajdaş, iki herkese açık Letterboxd profilinin film geçmişini karşılaştıran bir FastAPI uygulaması.

## Kurulum ve çalıştırma

Python 3.10 veya üzeriyle:

```sh
python -m pip install -r requirements.txt
python -m uvicorn main:app --reload
```

Tarayıcıda <http://127.0.0.1:8000> adresini açın.

## Kullanım

İki Letterboxd kullanıcı adı girin. Uyum skoru katalog örtüşmesine %35, ortak filmlerdeki puan benzerliğine %65 ağırlık verir. Sonuçta ortak film sayısını ve örnek filmleri de görebilirsiniz. Uygulama herkese açık profil sayfalarını okur ve erişim engellendiğinde sonuç üretemez.

## Proje yapısı

- `main.py` — FastAPI uygulaması, arayüz, profil ayrıştırma ve skor.
- `trivia.py` — bekleme ekranındaki sinema bilgileri.
- `requirements.txt` — Python bağımlılıkları.
