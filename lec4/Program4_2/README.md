# Вторая программа четвёртой лекции

Сначала программа создаёт массив файловых дескрипторов. После этого приложение проверит корректность ввода и сообщит об ошибке если нужно (14 и 20 строчки).
Затем программа вызовет fork() для получения PID'а дочернего процесса. Дальше приложение проверит только что полученный PID. У дочернего элемента этот идентификатор
равен нулю. Далее родительский процесс пишет что-либо в канал (42-49), а дочерний читает(34-42). Таким образом реализуется общение между процессами с помощью канала.
# Отладка
![Снимок экрана (165)](https://user-images.githubusercontent.com/104818494/169572931-077070b6-611d-4447-bc83-23e2858b7d61.png)
