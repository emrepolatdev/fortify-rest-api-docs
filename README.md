# Fortify REST API Docs

Fortify SSC REST API icin Postman collection ve entegrasyon dokumani.

## Postman Collection

Collection dosyasi:

```text
docs/Fortify SSC REST API - Basic To Advanced.postman_collection.json
```

Bu collection, Fortify SSC uzerinden proje/proje versiyonu secip vulnerability ve severity verilerini ucuncu parti sistemlere aktarmak icin hazirlanmistir.

## Authentication

Collection token degeri icermez. Musteri kendi SSC ortami icin token olusturup Postman variable olarak `fortifyToken` alanina girmelidir.

Token almak icin Postman'da `00 - Authentication - Create Token` request'i kullanilir.

Postman adimlari:

1. `Authorization` tab'ine gidin.
2. `Type = Basic Auth` secin.
3. SSC kullanici adini `Username`, SSC sifresini `Password` alanina girin.
4. Body icinde `AutomationToken` kullanin.
5. Response icindeki `data.token` degerini `fortifyToken` variable alanina yazin.

Token alma request'i `Basic Auth`, diger API request'leri `FortifyToken` kullanir.

Onerilen token tipi:

```json
{
  "type": "AutomationToken",
  "description": "Third-party integration token"
}
```
