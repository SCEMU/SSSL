![Screenshot_7](https://github.com/user-attachments/assets/8066723e-7279-498d-a0bf-82a0ffaa99a1)# **Практика №4 по предмету СДССиЛ - Network Threat Hunting**
Выполнил студент: Сидоренков Никита Дмитриевич 


Группы: ББМО-02-23

## **Шаг 1. Развертывание ВМ и запуск стенда:**
### **Скачанная и запущенная ВМ:**
![Снимок1](https://github.com/user-attachments/assets/f069082c-9723-4f96-af2e-eefd00c389fd)

### **Web-интерфейс развернутого стенда:**
![Снимок3](https://github.com/user-attachments/assets/6ee9b9bc-1610-4745-b627-7c1f986f5d72)

### **Выбор датасета для работы:**
![Снимок2](https://github.com/user-attachments/assets/87363ed8-f170-4614-98d7-6255fd0652fc)

### **Стартовая страница после аутентификации и выбора датасета развернутого стенда:**
![Снимок](https://github.com/user-attachments/assets/ed5175fe-82c7-4fe8-848d-ae1312efad3a)

### **Пример добавления адреса в safelist (skype.com):**
#### **Переходим в модуль beacons web:**
![Снимок4](https://github.com/user-attachments/assets/76fbef23-49c2-4807-b13e-5040da7c39b0)

#### **Выбор нужного адреса:**
![Снимок5](https://github.com/user-attachments/assets/17f01b57-03b0-4a9a-94dc-08a9cb8f30d6)

#### **Добавление адреса в safelist:**
![Снимок6](https://github.com/user-attachments/assets/e5528f49-43ec-415b-b3af-490a01a106db)

### **Проверка safelist на наличие добавленного ранее адреса:**
![Снимок7](https://github.com/user-attachments/assets/2c838ad1-d9ec-440e-8839-4f06db7799ca)

## **Шаг 2. Выполнение заданий из lab1:**
### **Переход в нужную директорию и импорт логов:**
![Снимок8](https://github.com/user-attachments/assets/1be78d2e-215f-4b90-877d-990d6c4c9b28)

### **Переключение на нужный датасет с загруженными ранее логами в web-итерфейсе:**
![Снимок9](https://github.com/user-attachments/assets/40c01eee-7126-494f-a885-27fd6abfb74a)

### **Стартовая страница с обнаруженными адресами и beacon score:**
![Снимок10](https://github.com/user-attachments/assets/7303c0e6-e9e3-4c62-b05d-645a5d206f0a)

### **Переход в beacons web для анализа адресов:**
![Снимок11](https://github.com/user-attachments/assets/25949ffc-df04-4660-b5c3-6ffaeaec14e9)

### **Проверка первого адреса:**
![Screenshot_1](https://github.com/user-attachments/assets/d289a73e-b437-418d-b5fd-ee1f1b929e21)

**Вывод по адресу** - Адрес проявляет подозрительную активность из-за количества подключений (3011), а также стабильности и прямолинейности графика зависимости количества подключений ко времени. Также не отображается полное доменное имя хоста, что может говорить о его вредоносности.

### **Проверка остальных адресов (для примера разберем 2 и 3 адреса):**
![Screenshot_7](https://github.com/user-attachments/assets/2102010c-f014-44af-b25f-50ea361cf279)
![Screenshot_8](https://github.com/user-attachments/assets/a7a4ca56-f0cc-4a33-9f4e-7e6a1fe1ef09)

**Вывод по адресам** - Два адреса и все последующие из списка относятся к компонентам и программам microsoft и вызывают доверие. Так же они не обладают большим количествам подключений. Из этого можно сделать вывод что данные адреса безопасны. Добавим по примеру, описанному выше, данные адреса в safelist

### **Проверка отображения добавленных ранее безопасных адресов в safelist:**
![Screenshot_9](https://github.com/user-attachments/assets/bbceac02-a6b9-4833-bcc0-e1e0e5f97961)














