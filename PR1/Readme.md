
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

## 3. Установким и настроим получения логов на сервер с использованием Loki

3.1 Установим и отредактируем docker compose файл на сервере
![Снимок11](https://github.com/user-attachments/assets/5b52932d-f7d0-476a-998e-5da2f65a9b36)

![Снимок16](https://github.com/user-attachments/assets/7141fc4a-5d6d-4929-baf0-75d9465a2d98)

3.2 Запускаем Loki
![Снимок14](https://github.com/user-attachments/assets/ae7f5bb0-7e4e-4ec5-b332-a576bb2e8940)

![Снимок18](https://github.com/user-attachments/assets/3c4139f3-11fc-44cd-9521-b64c5dadc79a)

3.3 Отредактируем promtail-config на клиенте
![Снимок19](https://github.com/user-attachments/assets/f953dab8-a9f6-44a0-b72e-d7e8ca5b2c6c)

3.4 Отредактируем docker compose файл для promtail
![Снимок16](https://github.com/user-attachments/assets/48dc4ae8-339a-4d56-ba23-e458344639a1)

3.5 Запустим promtail на клиенте
![Снимок20](https://github.com/user-attachments/assets/3fe3847c-fb93-4674-aa82-d45c4b92ee55)

3.6 Просмотрим логи клиента в Grafana Loki
![Снимок21](https://github.com/user-attachments/assets/1fd6f4e6-d687-47fd-870c-33df2ab01c70)

## 4 Настроим получения логов на сервере с использованием Signoz
4.1 Запускаем Singoz
![Снимок22](https://github.com/user-attachments/assets/585f4c14-7ebd-4b1e-88c5-6855bd619df6)

![Снимок23](https://github.com/user-attachments/assets/cfa844fd-80ae-491b-8f06-17094f46fe46)

![Снимок24](https://github.com/user-attachments/assets/6c38a3a6-5d9d-4bd9-870c-4dfc4a8834ec)

4.2 Отредактируем конфигурации на клиенте для отправки данных в Signoz
![Снимок25](https://github.com/user-attachments/assets/d720fcaf-1a1f-42ac-9817-a7d89da9b564)

4.3 Запустим клиентское приложение sample-nodejs-app
![Снимок27](https://github.com/user-attachments/assets/949cbd45-8d4d-4f3d-a106-1488d281ff86)

4.4 Проверим получение логов в Signoz
![Снимок26](https://github.com/user-attachments/assets/7599f58f-9ce5-44ed-9d67-08ea8582da0e)

![Снимок28](https://github.com/user-attachments/assets/a232bfad-25e7-43e4-b18d-0cd09ce15284)








