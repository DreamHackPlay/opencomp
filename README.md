# OpenComputers
Здесь собраны все мои программы, библиотеки для работы с OpenComputers, которыми я пользуюсь

#1. "Сумерки реактора"

Программа предназначена для мониторинга уровня заполненности буфера энергии в реакторе мода Big Reactors в Minecraft. Она автоматически считывает текущий уровень энергии и в зависимости от его значений управляет уровнями контроля стержней реактора.

Как работает программа:

Программа инициализируется с запросом на ввод максимальной емкости аккумулятора в реакторе (в RF/t).
После этого программа в режиме реального времени отслеживает уровень текущей заполненности аккумулятора, который варьируется от 0% до 100%.
В зависимости от заполненности аккумулятора программа плавно регулирует уровень стержней реактора: чем выше заполнение буфера, тем ниже опускаются стержни.
При полном заполнении аккумулятора стержни опускаются на 100%, что означает полное отключение реактора.
Когда уровень энергии в аккумуляторе начинает уменьшаться, программа поднимает стержни, уменьшая свою активность.
Функционал:

При старте программа запрашивает у пользователя максимальную емкость аккумулятора.
Далее, она отслеживает текущую заполняемость аккумулятора и вычисляет процентное соотношение заполненности.
В зависимости от этого процента программа изменяет уровень контроля над стержнями реактора:
0% заполнения — стержни полностью подняты.
100% заполнения — стержни полностью опущены.
Программа плавно изменяет положение стержней, пропорционально проценту заполнения буфера.
Программа продолжает работать в цикле, обновляя уровни стержней в зависимости от изменений в уровне энергии.
Программа позволяет безопасно и автоматизированно управлять уровнем стержней, предотвращая в пустую потраченные ресурсы на поддержание работы реактора.

Установка:
1. Установите OpenOS.
2. Запустите команду: wget 'https://raw.githubusercontent.com/DreamHackPlay/opencomputers/refs/heads/main/ReactorTwilight.lua' reactor.lua.
3. Скрафтите и установите в реактор "Компьютерный порт реактора".
4. Запустите программу, используя команду reactor.lua или reactor.
5. При первом запуске программа запросит у вас максимально возможное количество энергии в буфере реактора. В дальнейшем данные будут сохранены для повторных запусков.
6. Всё готово! Для выхода из программы нажмите "1".

Спасибо, что выбираете программы от "Волчары"
