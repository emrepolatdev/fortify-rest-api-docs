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

Onerilen token tipi:

```json
{
  "type": "AutomationToken",
  "description": "Third-party integration token"
}
```
