# Bot_Anekdot
Алгоритм. Подбор анекдотов состоит из трех этапов:
1. На первом ищем анекдоты по размеченным категориям.

2. Иначе ищем по совпадениям в предобработанном тексте.
В качестве ключевых слов оставляем существительные и прилагательные.

3. Иначе запускаем более глубокое сканирование
на основе косинусной близости по отобранным тэгам. Тэги отбираются на основе idf.
В качестве эмбэддингов используем предобученный FastText c rusvectores.
В данном случае, эти эмбэддинги оказались более качественными, чем эмбэддинги
русскоязычных бертов, которые мне удалось найти.
