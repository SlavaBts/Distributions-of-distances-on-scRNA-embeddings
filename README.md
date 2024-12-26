Задача в рамках курса по анализу данных single-cell-RNA-секвенирования. Охарактеризуйте характеристическое распределение расстояний внутри разных типов клеток на разных эмбеддингах: на экспрессиях (только на высоко вариабельных генах, отшкалированных и лог-трансформированных), на PCA, на UMAP, и на Palantir.

Файл **Euclidian_distances.ipynb** содержит построение распределений попарных евклидовых расстояния между точками в пространствах разных эмбеддингов при помощи модулей pdist и cdist.

Файл **kNN_distances.ipynb** содержит распределения расстояний только до k-ближайшиих соседей, посчитанных при помощи модуля sc.pp.neighbours на разных эмбеддингах. 
Описание основных файлов директории:
   
Основные этапы процессинга и анализа данных:

      - Загрузка данных (PBMC) и библиотек
      - Чтение данных 
      - Контроль качества клеток
      - Маркирование и удаление дублетов
      - Нормализация данных
      - Выделение гипервариабельных генов
      - Шкалирование (построение эмбеддинга Z-статистик - он же экспрессионный эмбеддинг) 
      - PCA
      - UMAP
      - Palantir
      - Построение и визуализация различных распредеелений 
