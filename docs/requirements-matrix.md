## Матрица
| Требование ЛР1 | Поле или сущность | Запрос | Критерий |
|----------------|-------------------|--------|----------|
| Создать объект | `Contract`, `number`, `conclusion_date`, `end_date`, `type`, `status`, `supplier`, `customer`, `payment_terms`, `description` | `POST /api/contracts` | 1 |
| Назначить исполнителя | `assigneeEmployeeId` | `PATCH …/assignee` | 2 |
| Перевести в работу | `status` | `PATCH …/status` | 3 |