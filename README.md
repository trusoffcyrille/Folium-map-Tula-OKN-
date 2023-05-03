Folium-map-Tula-OKN-

БГП193: Азовцева Татьяна, Ураскина Екатерина, Трусов Кирилл, Яковская Мария

Веб-карты: интерактивное отображение объектов культурного наследия

Для выполнения данной задачи нами был выбрал город Тула. Для того, что погрузиться в анализ находящихся там объектов культурного наследия (далее ОКН) мы провели небольшой исторический и пространственный анализ территории.

Тула, родина оружия, пряников и самоваров - город в 185 км от Москвы, история которого насчитывает более 870 лет. Он является административным центром Тульской области и Городом-героем (c 1976 года), располагается на севере Среднерусской возвышенности на берегу реки Упы. На 2021 год в Туле проживает около 470 тыс. жителей.

Площадь города составляет 1 495 км². Сам же город внутри делится на Зареченский, Привокзальный, Пролетарский, Советский и Центральный районы. На территории города имеется более 300 объектов культурного наследия: это памятники архитектуры и градостроительства, истории, археологии, произведения монументального искусства, также сохранилось много старинных зданий XVIII-XIX века. Самые известные достопримечательности, визитные карточки города - Тульский кремль, Музеи главных символов города: Тульского пряника, оружия и самоваров, Успенский кафедральный собор, Памятник Левше и другие.

Данные для данной работы были выгружены с "Реестра объектов культурного наследия", а если быть точнее с официального сайта Инспекции Тульской области по государственной охране объектов культурного наследия". Файл находится в открытом доступе, поэтому его загрузка не вызвала у нас проблем.

Ссылку на источник прилагаем: https://okn.tularegion.ru/okhrana-naslediya/reest-obektov-kulturnogo-naslediya/

Данные по границам города и его внутреннему административному делению были выгружены также из открытых источников - через плагин QuickOSM, ранее установленный в QGIS.

Для создания интерактивной карты нами была использована библиотека Folium для Python. Изначально информация по ОКН была выгружена в формате точек. Поэтому при создании полигонального слоя зданий информация была взята из соответствующих точек. Также поскольку данная выгрузка была по Тульской области была произведена фильтрация и выбраны точки только в границах города. Кластеризация точек была проведена через MarketClaster. Далее была создана регулярная сеть для агрегации точечного слоя ОКН, и в ней также было подсчитано количество точек.

По итогам работы удалось настроить интерактивную карту по городу Тула с уникальным набором данных, содержащих информацию по всем установленным законодательством ОКН в пределах городского округа. Однако не получилось выполнить более тонкие настройки стилей для визуализации для каждого слоя (например, прозрачность для внутренней области). Но здесь уже вопрос визуальной составляющей данной работы.

Стоит отметить, что в процессе работы все было не так гладко, поэтому сложности возникли в:

настройке визуализации данных через код
работе с проекциями при настройке интерактивной карты
обработке данных по ОКН
Для отображения конечного результата работы прикладываем ссылку на нашу веб-карту: file:///C:/Users/yakow/Downloads/Telegram%20Desktop/index.html
