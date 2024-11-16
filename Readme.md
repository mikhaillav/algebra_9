# Конспект по алгебре 9 класса

Красивый конспектик по алгебре.

## Содержание

- Степени и корни
    - Степень с целым показателем
    - Арифметический корень натуральной степени
    - Свойства корня натуральной степени
    - Степень с рациональным показателем
    - Свойства степени с рациональным показателем
- Графики и Функции
    - Обратная функция
    - Свойства и графики степенной функции
        - Натуральная нечетная степень
        - Натуральная четная степень
        - Привет, это Гипербола
        - Четная целая отрицательная степень
        - Корень нечетной степени
        - Корень четной степени
- Иррациональность
    - Иррациональные уравнения
    - Иррациональные неравенства

## Использование

Все начинается с [main.tex](main.tex), там лежат зависимости, там можно настроить оформление, окружение и прочее.
Там же можно поправить титульный лист и аннотацию.
Конспект состоит из содержания и глав, они, по задумке лежат в папке [tex](./tex/). 

Что делают файлы из примера:
- [main.tex](main.tex) - основный файл, включает в себя все главы
- [contents.tex](./tex/contents.tex) - код содержания, лучше не трогать
- [chapter_1](./tex/chapter_1/) - папка с первой главой
- [chapter_1.tex](./tex/chapter_1/chapter_1.tex) - код первой главы, содержит оглавление и включает в себя файлы секций
- [section_1.tex](./tex/chapter_1/section_1.tex) - код первой секции первой главы, вот там надо писать буковки
- [chapter_1/assets](./tex/chapter_1/assets/) - папка с медиа, у каждой главы она своя, хотя, делайте как хотите

В проекте есть свой [Makefile](Makefile), написанный для `pdflatex`. 
Используя его, собрать проект можно командой `make`, результат будет в папке `build`.
Очистить файлы сборки можно командой `make clean`.

Если вы используете не `pdflatex`, желаю вам удачи в сборке :)
Возможно, проект не соберется или соберется не сразу =)