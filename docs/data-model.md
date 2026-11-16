![Alt text](<Схема БД СКИД 3.PNG>)



| Термин курса | Термин моей темы |
|--------------|------------------|
| Order | заявка |
| Contract | договор |
| Employee | сотрудник отдела |

Главный объект (contract) содержит поля: id, number, conclusion_date, end_date, type, status, supplier, customer, employee_id, total_amount, payment_terms, description, created_at, updated_at

Справочник (order) содержит поля: id, number, address, start_date, end_date, contract_id

У пользователя (employee): id, full_name, position

## Проверка 3НФ
Order содержит внешний ключ contract_id, который является внешним ключом на поле id сущности contract. 






