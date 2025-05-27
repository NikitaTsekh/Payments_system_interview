# 💳 Payments System — Django Interview

🧪 Тестовое задание для Backend Django Developer

---

## 📦 Задача: имитация webhook от банка

Реализовать backend-сервис, который:

- принимает входящие webhook-и от банка
- обрабатывает их
- корректно начисляет баланс организации по ИНН

---

## 🔧 Технологии

- Python 3.9  
- Django 4.2.17  
- MySQL

---

## 📥 POST `/api/webhook/bank/`

Webhook принимает JSON следующего формата:

```json
{
  "operation_id": "ccf0a86d-041b-4991-bcf7-e2352f7b8a4a",
  "amount": 145000,
  "payer_inn": "1234567890",
  "document_number": "PAY-328",
  "document_date": "2024-04-27T21:00:00Z"
}
