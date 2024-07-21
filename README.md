1_7

Описание
Флэш-карта — это цифровая или бумажная карточка, которая содержит термин на одной стороне и определение, перевод или объяснение этого термина на другой. Флэш-карты часто используются для изучения иностранных языков и являются эффективным методом обучения для многих людей.

Карточка: верхняя часть — термин, который задают пользователю, нижняя часть — правильный ответ.

Пример карточки. Верхняя часть — термин, который спрашивают у пользователя, нижняя часть — правильный ответ. Источник: Википедия .

В этом проекте мы будем называть текст на лицевой стороне карточки термином, а текст на обороте — определением. На самом деле не будет визуальной «лицевой» и «обратной» стороны карточки: все будет сделано с помощью последовательного текста. Мы попросим пользователя дать определения ранее введенным терминам и проверим правильность данных ответов. Разрабатывая это приложение, вы не только научитесь программированию, но и сэкономите бумагу!

Цели
Ваша программа должна считывать с консоли две строки: термин и определение, представляющие карту.

Реализуйте программу, которая выводит 4 строки:

Первая строка —Card:
Вторая строка — термин, предоставленный пользователем.
Третья строка —Definition:
Четвертая строка — определение, которое также предоставлено пользователем.
На этом этапе мы только закладываем фундамент для последующих этапов, мы начнем использовать эти входные значения со следующего этапа.

Примеры
Вот несколько примеров вывода, чтобы прояснить, как должен выглядеть результат. Символ «больше», за которым следует пробел ( > ), представляет собой пользовательский ввод. Обратите внимание, что он не является частью ввода.

Пример 1.

Card:
> purchase
purchase
Definition:
> buy
buy

Пример 2.

Card:
> cos'(x)
cos'(x)
Definition:
> -sin(x)
-sin(x)

2_7

Описание
На этапе 1 мы узнали, как создать динамическую карточку из пользовательского ввода. Давайте также добавим примитивный механизм угадывания, чтобы пользователь мог проверить, насколько хорошо он помнит определения.

На этом этапе вы расширите механизм создания карточек, реализованный на этапе 1, и добавите поверх него функционал для проверки ответа пользователя.

Цели
Подобно этапу 1, ваша программа должна прочитать две строки с консоли, термин и определение, которые представляют карту. Однако на этом этапе нет необходимости печатать Card:или .Definition:

После этого пользователь вводит строку в качестве ответа (определение термина на карточке). Сравните ответ пользователя с правильным определением и выведите результат.

Результатом работы программы должен быть один из следующих:

Your answer is wrong...если ответ не соответствует определению;
Your answer is right!если ответ соответствует определению.
Конечно, на этом этапе пользователь вряд ли даст неправильный ответ, поскольку он только что ввел ответ... Но не волнуйтесь: сейчас мы просто разминаемся, чтобы на более поздних этапах немного усложнить задачу для наших пользователей.

Примеры
Символ "больше" с последующим пробелом ( > ) представляет собой пользовательский ввод. Обратите внимание, что он не является частью ввода.

Пример 1: ответ пользователя правильный

Ввод (термин, затем определение и, наконец, ответ):

> print()
> outputs text
> outputs text

Выход:

Your answer is right!

Пример 2: ответ пользователя неверный

Ввод (термин, определение, ответ):

> Jetbrains
> A place for people who love to code
> A place for people who hate to code

Выход:

Your answer is wrong...

3_7

Описание
Ваша программа может развлекать пользователей только одной картой, что не очень весело. Давайте выведем нашу игру на новый уровень и реализуем набор карточек.

Позвольте пользователю решить, сколько карточек он хотел бы сделать. Сначала попросите игрока ввести желаемое количество карточек. Затем попросите его ввести термин и определение для каждой карточки.

В конце концов, как только все карточки будут определены и сохранены, ваша программа наконец-то готова к использованию в качестве игры! Спросите игрока обо всех новых словах, которые он ввел. Программа должна выдать термин и попросить его определение.

Цели
Ваша программа должна выполнять следующие действия:

Получите количество карточек, которые пользователь хотел бы создать. Для этого выведите строку Input the number of cards:в качестве подсказки для пользователя, а затем прочитайте число из следующей строки.
Создайте определенное количество карточек в цикле. Чтобы создать карточку, выведите строку , где n — индексный номер карточки, которую нужно создать; затем считайте введенные пользователем данные (термин) из следующей строки. Затем выведите строку и считайте определение термина пользователем из следующей строки. Повторяйте, пока не будут созданы все карточки.Card #n:The definition for card #n:
Проверьте пользователя на знание определений всех терминов в том порядке, в котором они были добавлены. Чтобы сделать это с одной карточкой, выведите строку, где находится термин карточки, который нужно проверить, а затем прочитайте ответ пользователя со следующей строки. Обязательно поместите термин карточки в кавычки. Затем выведите строку, если ответ пользователя правильный, или строку , если ответ неправильный, где находится правильное определение. Повторите для всех карточек в наборе.Print the definition of "term":"term"Correct!Wrong. The right answer is "definition"."definition"
Пример
Символ > представляет собой пользовательский ввод. Обратите внимание, что он не является частью ввода.

Input the number of cards:
> 2
Card #1:
> print()
The definition for card #1:
> outputs text
Card #2:
> str()
The definition for card #2:
> converts to a string
Print the definition of "print()":
> outputs text
Correct!
Print the definition of "str()":
> outputs text
Wrong. The right answer is "converts to a string".

Обратите внимание, что все ваши выходные данные и пользовательские вводы должны располагаться на отдельных строках.

4_7

Описание
Изучая новые вещи, мы можем перепутать вещи и использовать правильное определение для неправильного термина. Давайте сообщим нашим игрокам, если они введут неправильное определение для запрошенной карточки, но исправят его для другой карточки в нашем наборе.

Также, это может быть очень запутанным, если наш набор карточек содержит карточки с одним и тем же термином или определением, поскольку, видя только одну сторону карточки, мы не можем их различить. Давайте добавим ограничение: пользователь должен добавлять только уникальные термины и определения. Для этого вам нужно найти способ проверить, содержит ли набор определенный термин или определение, и получить термин по определению, и наоборот.

Эти две функции определенно улучшат нашу игру!

Цели
Измените вашу программу так, чтобы она вела себя следующим образом:

Если пользователь пытается добавить дублирующийся термин, запретите это и выведите сообщение, используя термин вместо . Спрашивайте термин, пока пользователь не введет уникальный термин.The term "term" already exists. Try again:"term"
Когда пользователь пытается добавить дубликат определения, запретите это и выведите сообщение с определением вместо . Попросите игрока ввести определение, пока пользователь не введет уникальное.The definition "definition" already exists. Try again:"definition"
Если пользователь вводит неверное определение для запрошенного термина, но это определение верно для другого термина, выводится соответствующее сообщение , где — фактическое определение для запрошенного термина, а — подходящий термин для введенного пользователем определения.Wrong. The right answer is "correct answer", but your definition is correct for "term for user's answer"."correct answer""term for user's answer"
Примеры
Символ > представляет собой пользовательский ввод. Обратите внимание, что он не является частью ввода.

Пример 1: пользователь пытается добавить дублирующийся термин и определение

Input the number of cards:
> 2
Card #1:
> print()
The definition for card #1:
> outputs text
Card #2:
> print()
The term "print()" already exists. Try again:
> str()
The definition for card #2:
> outputs text
The definition "outputs text" already exists. Try again:
> converts to a string
Print the definition of "print()":
> outputs text
Correct!
Print the definition of "str()":
> converts to a string
Correct!

Пример 2: пользователь дает правильное определение термину, который существует, но не является термином, о котором спрашивает программа.

Input the number of cards:
> 2
Card #1:
> uncle
The definition for card #1:
> a brother of one's parent
Card #2:
> ankle
The definition for card #2:
> a part of the body where the foot and the leg meet
Print the definition of "uncle":
> a part of the body where the foot and the leg meet
Wrong. The right answer is "a brother of one's parent", but your definition is correct for "ankle".
Print the definition of "ankle":
> ???
Wrong. The right answer is "a part of the body where the foot and the leg meet".

Обратите внимание, что все ваши выходные данные и пользовательские вводы должны располагаться на отдельных строках.

5_7

Input the action (add, remove, import, export, ask, exit):
> add
The card:
> a brother of one's parent
The definition of the card:
> uncle
The pair ("a brother of one's parent":"uncle") has been added.

Input the action (add, remove, import, export, ask, exit):
> add
The card:
> a part of the body where the foot and the leg meet
The definition of the card:
> ankle
The pair ("a part of the body where the foot and the leg meet":"ankle") has been added.

Input the action (add, remove, import, export, ask, exit):
> ask
How many times to ask?
> 6
Print the definition of "a brother of one's parent":
> ankle
Wrong. The right answer is "uncle", but your definition is correct for "a part of the body where the foot and the leg meet".
Print the definition of "a part of the body where the foot and the leg meet":
> ??
Wrong. The right answer is "ankle".
Print the definition of "a brother of one's parent":
> uncle
Correct!
Print the definition of "a part of the body where the foot and the leg meet":
> ankle
Correct!
Print the definition of "a brother of one's parent":
> ??
Wrong. The right answer is "uncle".
Print the definition of "a part of the body where the foot and the leg meet":
> uncle
Wrong. The right answer is "ankle", but your definition is correct for "a brother of one's parent".

Input the action (add, remove, import, export, ask, exit):
> exit
Bye bye!

6_7

Статистика
Описание
Во время обучения может быть очень полезно уделять больше внимания сложным частям, где вы делаете больше всего ошибок. На этом этапе вы добавите в свою программу некоторые статистические функции, чтобы пользователи могли отслеживать свой прогресс.

Реализовать следующие дополнительные действия:

сохранить журнал приложения в указанный файл:log

выведите термин или термины, в которых пользователь допускает больше всего ошибок:hardest card

сотрите количество ошибок для всех карт:reset stats

Помните, что теперь вам нужно хранить три элемента (термин, определение, ошибки) вместо двух (термин, определение).

Цели
Выводить сообщение Input the action (add, remove, import, export, ask, exit, log, hardest card, reset stats):каждый раз, когда пользователю предлагается выполнить следующее действие. Действие считывается со следующей строки, обрабатывается, и сообщение выводится снова, пока пользователь не решит выйти из программы.

Поведение программы зависит от входных действий пользователя:

log— спросить пользователя, куда сохранить журнал с сообщением File name:, сохранить все строки, которые были введены/выведены на консоль, в файл и вывести сообщение The log has been saved.Не очищайте журнал после сохранения в файл.

hardest card— вывести строку, содержащую термин карточки с наибольшим количеством неправильных ответов, например, The hardest card is "term". You have N errors answering it.Если есть несколько карточек с наибольшим количеством неправильных ответов, вывести все термины: The hardest cards are "term_1", "term_2". Если карточек с ошибками в ответах пользователя нет, вывести сообщениеThere are no cards with errors.

reset stats— установить количество ошибок на 0 для всех карточек и вывести сообщениеCard statistics have been reset.

Обновите свои действия importи exportдействия с предыдущего этапа, чтобы количество ошибок для каждой карточки также импортировалось и экспортировалось.

Пример
Символ > представляет собой пользовательский ввод. Обратите внимание, что он не является частью ввода.

Input the action (add, remove, import, export, ask, exit, log, hardest card, reset stats):
> hardest card
There are no cards with errors.

Input the action (add, remove, import, export, ask, exit, log, hardest card, reset stats):
> import
File name:
> capitals.txt
28 cards have been loaded.

Input the action (add, remove, import, export, ask, exit, log, hardest card, reset stats):
> hardest card
The hardest card is "France". You have 10 errors answering it.

Input the action (add, remove, import, export, ask, exit, log, hardest card, reset stats):
> ask
How many times to ask?
> 1
Print the definition of "Russia":
> Paris
Wrong. The right answer is "Moscow", but your definition is correct for "France" card.

Input the action (add, remove, import, export, ask, exit, log, hardest card, reset stats):
> hardest card
The hardest cards are "Russia", "France". You have 10 errors answering them.

Input the action (add, remove, import, export, ask, exit, log, hardest card, reset stats):
> reset stats
Card statistics have been reset.

Input the action (add, remove, import, export, ask, exit, log, hardest card, reset stats):
> hardest card
There are no cards with errors.

Input the action (add, remove, import, export, ask, exit, log, hardest card, reset stats):
> log
File name:
> todayLog.txt
The log has been saved.

Input the action (add, remove, import, export, ask, exit, log, hardest card, reset stats):
> exit
Bye bye!

7_7

Описание
Файлы используются для сохранения прогресса и его восстановления при следующем запуске программы пользователем. Утомительно распечатывать действия вручную. Иногда вы можете просто забыть это сделать! Давайте добавим аргументы запуска, которые определяют, какой файл читать в начале и какой файл сохранять при выходе.

Цели
При наличии аргументов командной строки ваша программа должна выполнить следующие действия:

Если -import IMPORTпередано, где IMPORT имя файла, прочитать начальный набор карт из внешнего файла и вывести сообщение n cards have been loaded.в качестве первой строки вывода, где nколичество загруженных из внешнего файла карт. Если такой аргумент не указан, набор карт изначально должен быть пустым и сообщение о загрузке карты не должно выводиться.
Если -export EXPORTпередано , где EXPORT— имя файла, записать в этот файл все карточки, которые находятся в памяти программы после ввода пользователем exit, а последняя строка вывода должна быть n cards have been saved., где n— количество карточек в наборе.
Примеры аргументов запуска
java Flashcards -import derivatives.txt

java Flashcards -export animals.txt

java Flashcards -import words13june.txt -export words14june.txt

java Flashcards -export vocab.txt -import vocab.txt 
