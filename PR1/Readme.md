
# СДССиЛ Практическая работа номер 1 - Аггрегация и сбор логов
Выполнил - Сидоренков Никита Дмитриевич

## 1. Создаем 2 виртуальные машины на базе ОС Debian 12 и обеспечиваем между ними сетевой обмен (Использовался VirtualBox как клиент виртуализации):
![Снимок1](https://github.com/user-attachments/assets/c455fdce-aeba-49ea-b08f-0c2064a58f4d)
![Снимок2](https://github.com/user-attachments/assets/0bbcc58d-1725-4fa0-aeb6-cd8fd968b941)
![Снимок5](https://github.com/user-attachments/assets/4f42d872-91e4-49bd-8fc6-a5bcb1692400)

## 2. Включаем на 1-ой (сервере) из ВМ передачу логов по протоколу rsyslog на 2-ую ВМ (клиент):
2.1 Устанавливаем и настраиваем rsyslog на сервере и клиенте:
![Снимок6](https://github.com/user-attachments/assets/f9a1e4ae-52ad-446b-aab2-a8ce106bf5b4)

2.2 Проверяем работоспособность rsyslog на сервере и клиенте:
![Снимок7](https://github.com/user-attachments/assets/a53cac47-e617-46e3-a859-c41c3eaba559)

2.3 Включим UDP и TCP соединения
![Снимок8](https://github.com/user-attachments/assets/115a1fff-428b-44b5-8a75-abb3b0e56540)

2.4 Установим правила на сервере и клиенте
![Снимок9](https://github.com/user-attachments/assets/a3534364-8af0-4c49-882a-840a361ec8f6)

2.5 Проверим получения логов на сервере
![Снимок10](https://github.com/user-attachments/assets/5023821c-902a-4fcb-a3a1-bb0ee02e34e3)
