    `В крупном дейтинговом приложении, помимо базовых функций, также имеется премиум-подписка, которая дает доступ к ряду важных дополнительных возможностей.
    В ходе A/B тестирования некоторой гипотезы целевой группе была предложена новая стоимость премиум-подписки для новых пользователей из нескольких стран при покупке через две новые платежные системы. При этом стоимость пробного периода премиум-подписки оставалась прежней.
    У контрольной группы условия премиум-подписки не изменялись. Необходимо проанализировать итоги эксперимента и сделать вывод, стоит ли запускать новую стоимость услуги на всех пользователей.
    
### ПЛАН РАБОТЫ:
1.	Определение метрик для проверки успешности эксперимента
2.	Загрузка данных, проверка данных в датасете, предобработка данных
3.	Проверка выборок на репрезентативность
4.	А/А тестирование. Проверка системы сплитования
5.	А/В тестирование
6.	Вывод: был ли эксперимент успешен.

### 1.	Определение метрик
Так как целевой группе была предложена новая стоимость услуги на сайте, то в первую очередь это повлияет на конверсию пользователя в премиум пользователя (CR). Именно эту метрику возьмем за основу для выводов.
Сопутствующие метрики, которые можно отследить, чтобы они не падали: средняя выручка всех пользователей сайта(ARPU), средняя выручка премиум пользователей (ARPPU).

### 2.	Загрузка данных, проверка данных в датасете, предобработка данных
В результате предобработки сформирован датасет, в котором:
-	данные загружены, прочитаны, проверены типы данных, наличие дубликатов.
-	определены три группы пользователей (тестовая и две контрольных) (регистрация в период эксперимента с 11.01.2017 по 31.10.2017); 
-	отобраны данные из тех стран,где проводилось исследование (страны в контрольных группах совпадают с тестовой); 
-	каждому пользователю добавлена сумма его трат в первую очередь на подписку Премиум, на пробную подписку и на остальные продукты. 
Таким образом, датасет, с которым в дальнейшем буду проводить анализ предобработанных данных users готов.

### 3.	Проверка выборок на репрезентативность
Посмотрим на количество пользователей. Почти одинаковое количество во всех группах: 

Распределение по гендеру: 




