Скачайте все необходимые файлы из репозитория, включая скрипт Practice.py и папку с журналами доступа и настройками.
Убедитесь, что у вас установлены Python, Flask, sqlite3 и apache_log_parser.
Проверьте, что порт 5000 свободен для использования.
Запустите скрипт через командную строку командой: python -i Practice.py.
Используйте функцию parse_logs(путь_к_файлу_с_логами) для заполнения базы данных.
Для просмотра журналов в базе данных используйте команду view_logs. Чтобы увидеть все логи, введите: view_logs().
Если необходимо выполнить поиск журналов по конкретным параметрам, используйте: view_logs(date_from, date_to, ip, status). Например: view_logs('дата от', 'дата до', 'ip', статус).
Для получения данных в формате JSON используйте функцию generate_get_logs_link(). Для получения всех данных введите: generate_get_logs_link() и обратите внимание на сгенерированную ссылку.
Чтобы выбрать определенные журналы, используйте те же аргументы, что и для view_logs, но в формате словаря. Пример: generate_get_logs_link({'date_from':'дата от', 'date_to':'дата до', 'ip':'ip', 'status':статус}), затем проверьте результат по сгенерированной ссылке.
