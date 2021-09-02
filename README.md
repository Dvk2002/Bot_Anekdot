# Bot_Anekdot
Алгоритм. Подбор анекдотов состоит из трех этапов:
На первом ищем анекдоты по размеченным категориям.
Иначе ищем по совпадениям в пред обработанном тексте.
В качестве ключевых слов оставляем существительные и прилагательные.
Иначе запускаем более глубокое сканирование
на основе косинусной близости по отобранным тэгам.
В качестве эмбэддингов используем предобученный FastText c rusvectores.
В данном случае, эти эмбэддинги оказались более качественными, чем эмбэддинги
русскоязычных бертов, которые мне удалось найти.
