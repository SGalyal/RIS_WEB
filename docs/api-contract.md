## API
| Метод и путь | Тело | Успех | Возможная ошибка |
|--------------|------|-------|------------------|
| `GET /api/contracts` | — | `200`, массив или `[]` | — |
| `GET /api/contracts/{id}` | — | `200`, объект | `404` |
| `POST /api/contracts` | `number`, `conclusion_date`, `end_date`, `type`, `status`, `supplier`, `customer`, `payment_terms`, `description` | `201`, `id`, `status: New` | `400` |
| `PATCH /api/contracts/{id}/assignee` | `assigneeEmployeeId` | `200` | `404` |
| `PATCH /api/contracts/{id}/status` | `status` | `200` | `404`, `409` |