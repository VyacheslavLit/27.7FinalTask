# 27.7FinalTask
1.	Требования к работе.
Для запуска необходимо скомпилировать отдельно 2 программы сервер и клиент, а также импортировать приложенный dump базы.
База данных сформирована в MySQL.
Dump базы произведен с помощью MySQLWorkbench.

2.	Пояснения к работе.
Добавлен класс Logger.
Класс Logger предоставляет 2 метода, getLog и setLog. В их тела прописаны мьютексы.
В тело метода zaprosMySQL класса Server добавлен новый поток с вызовом метода setLog, обеспечивающий сохранение всех запросов, пока zaprosMySQL продолжает выполняться.
