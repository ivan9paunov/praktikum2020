# praktikum2020

Здравейте, прикачил съм проекта си с наименование „Филмов проект“.

За реализацията е използвано следното API:
https://www.themoviedb.org/documentation/api?language=en-US

Графичният интерфейс има следната функционалност:
Избор на година, сортиране по критериите „популярност“ и „най-висок рейтинг“. Търсенето по жанр и съответно визуализирането на върнатите резултати не съумях да го осъществя.

В основния home.html файл е изпълнен request-а:
https://api.themoviedb.org/3/discover/movie?year=2020&api_key=f1f5877c7d8c646b47bf279e9130fdd1

От него се зареждат най-популярните филми за 2020 година, като съм визуализирал заглавието на филма, датата му на излизане, рейтинг и описание, което е видимо при натискане върху бутона „РЕЗЮМЕ“. При него не успях да разреша проблема, който показва описанието (също и заглавието) на първия филм при всички следващи, а не техните (вероятно защото е в допълнителен Modal). Опитах да добавя и жанр, но трябва да използвам друг request, а не успях да разбера с каква функция се използват два (или повече) линка в един документ. Изкоментирал съм в същия файл под зареждането на филмите един код, при който успявам да заредя имената на жанровете (вътре в modal), но другите елементи не се визуализират (снимка, заглавие, ..).

Съответно затова са и файловете home-search, home-sortByCriterion и home-sortByYear. Пак поради незнанието как да бъдат използвани два линка в един документ. При home-search работи единствено функцията за търсене по име на филм (опитайте с някое заглавие – Batman, Titanic или други). Бутона „ИЗЧИСТИ“ съм го сложил, защото при търсене на друг филм, резултатите се визуализират под предишните. Смятам, че това е заради append метода, но не знам onclick функция ли трябва да използвам, или какво.. Затова го направих първобитно, но функциониращо чрез бутона изчисти. Другите 2 sort файла са съответно за падащите менюта и също работят чрез бутоните „ИЗЧИСТИ“ и „ТЪРСИ“.

Като обобщение - проблемите ми са в това да използвам няколко request-а в един файл и да визуализирам новата информация върху предходната, а не append-ната под нея.
Изпращам Ви го в този вид, като към момента това са възможностите ми. Търсих из интернет и изпробвах различни опции да събера функционалностите в един файл, но докато не науча JS функциите няма да се получи. Ще се радвам след като оцените проекта, ако може да ми преправите кода да функционират търсене/сортиране само от home.html, като по default винаги да показва най-популярните, пък аз ще си анализирам нещата след това сам.

*Също така каква е причината да се показват резултатите в modal-а само за първия филм?
