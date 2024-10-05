1) Перед запуском убедитесь, что в корневой папке с Jupiter notebook созданы папки \input_data и \output_data

2) В папку \input_data загрузите с Kaggle файлы с данными events.csv, item_properties_part1.csv, item_properties_part2.csv по ссылке: 
https://www.kaggle.com/datasets/retailrocket/ecommerce-dataset?resource=download&select=category_tree.csv
или 
kaggle datasets download -d retailrocket/ecommerce-dataset

3) RFD_main.ipynb представляет исследование данных о покупателях с оформлением RFD таблицы, где:
	Recency - свежесть: количество дней с последней покупки
	Frequency - частота: количество покупок за весь измеряемый период
	Duration - продолжительность: суммарная продолжительность периодов действий покупателей, промежуток между 		которыми < control_period

4) RFD_train_test.ipynb представляет исследование данных о покупателях с оформлением двух RFD таблиц за разные временные периоды в целях проверки гипотезы,  
   что  покупатели с хорошим RFD рейтингом в прошлом будут и в будущем лояльными покупателями (рейтинг RFD_test >= RFD_train): 
	RFD_train - RFD таблица за первый период времени.
	RFD_test - RFD таблица за последующий период времени.

5) Дополнительные инструкции и пояснения указаны в Jupiter notebook