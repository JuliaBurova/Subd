**Введение**
=====================
Система, разрабатываемая командой, поможет упростить процесс работы диспетчера кассы автовокзала.
***
В системе собрана информация о различных маршрутах, откуда и в каком направлении они осуществляются. Также там располагается информация о проданных билетах. Диспетчера могут вносить всю необходимую информацию обновленную информацию. Различные транспортные средства (автобус, маршрутное такси) имеют свои маршруты и диспетчер сам выбирает, что именно его интересует. Упрощение просмотра и выбора маршрута представляет интерес для пользователей данного сайта.
***
База данных «Автоматизация работы диспетчера» создается для экономии времени, которое тратится на составление маршрутов об имеющихся направлениях. 
***
### Задача: разработать СУБД, которая позволит упростить работу диспетчеров, отвечающую за учет направлений и помогающую диспетчерам продавать билеты. Описываемый прототип позволит хранить информацию о транспортах, водителях, маршрутах.  
***
**Предметная область**
=====================
Основные идеи современной информационной технологии базируются на концепции, согласно которой данные должны быть организованы в базы данных с целью адекватного отображения изменяющегося реального мира и удовлетворения информационных потребностей пользователей. Эти базы данных создаются и функционируют под управлением специальных программных комплексов, называемых системами управления базами данных (СУБД).
***
### Предметная область: процесс учета данных о различных маршрутах и продаже билетов.
***
**Функциональные требования**
=====================
1. Пользователю должен быть доступен выбор различных баз данных.
2. В соответствии с типом пользователя должны быть разграничены права.Обеспечивать доступ к редактированию таблиц "Изделия", "Материалы" только типу пользователя "Компания".Обеспечивать доступ к редактированию таблиц "Заказ материалов", "Заказ изделий" только типу пользователя "Покупатель".
3. К просмотру данных должен иметь доступ любой посетитель сайта, вне зависимости от его типа.
4. Удаление записей должно регулироваться, чтобы не было нарушения целостности.
***
**Нефункциональные требования**
=====================
1. Осуществляя переключение по кнопкам в верхней части сайта пользователь сменяет базы данных. 
2. Просматривать данные можно попадая на сайт.
3. Удаление осуществляется по кнопке, но если у Базы данных есть подозрения в правильности вашего выбора, то выдается предупреждение.
4. В БД существует поиск необходимого маршрута по введенным словам-подсказкам, например, имя водителя.
5. Редактирование осуществяется только диспетчерами.
***
Для составления данных потребуется информация о маршрутах: его номер, время отправки, пункте отправления и прибытия, расстоянии. Данные о водителях должны содержать сведения о ФИО, паспортные данные и дату рождения. 
Для составления отчетной ведомости потребуется информация о поступлениях материалов, их количества, цене. Данные о клиентах должны содержать сведения о фамилии, логине, пароле. Данные о заказе базируются на основе номера услуги, номера материала, количестве.
***
В БД есть данные и о транспорте автобусе или маршрутном такси – его номер, модель и вместимость. Также будут данные о самой перевозке, где будет храниться хранится информация с номером маршрута, билетом, данными диспетчера, который заносит перевозку в БД, транспортом и водителем.
***
**Макеты предполагаемого интерфейса**
=====================
[Макет 1](https://drive.google.com/open?id=1LHdDH8ZFGGFcVJmsj_O4-zjl_zyQnTnT)
##### Макет 1
***
[Макет 2](https://drive.google.com/open?id=1FAP3NUgTs5lc-iFKKbbkLjx1_K8gGz2s)
##### Макет 2
***
[Макет 3](https://drive.google.com/open?id=14EeQfFOUYp0r5gc_EdpA82mHld31qc_D)
##### Макет 3
***
##### Описание хранимых данных в каждой из используемых БД
***
[Диаграмма 1](https://erdplus.com/#/edit-diagram/885004)
***
##### Взаимодействие между водителем и пассажиром
***
[Диаграмма 2](https://www.draw.io/#G1BdTl5ZRJ-YnGAskvqAHTiqtlq2-gYG8o)
***
##### ER-диаграмма
***
[Диаграмма 2](https://erdplus.com/#/edit-diagram/885020)
***
##### Подробная диаграмма
***
[Диаграмма 3](https://my.vertabelo.com/public-model-view/oV00MW0WqAYw0zR4oPMDGe2s0vWRqc2bhvxv08JnWdaL9tpUw7qOqSH3W96b5TUx?x=-642&y=513&zoom=0.1571)
# Subd
