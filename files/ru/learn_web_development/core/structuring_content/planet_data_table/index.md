---
title: "Аттестация: Структурирование данных о планетах"
slug: Learn_web_development/Core/Structuring_content/Planet_data_table
---

{{LearnSidebar}}{{PreviousMenu("Learn/HTML/Tables/Advanced", "Learn/HTML/Tables")}}

В нашей аттестации, мы предоставим вам некоторые данные о планетах солнечной системы, и убедим вас структурировать их в HTML таблицу.

| Необходимые навыки: | Перед тем, как попытаться пройти эту аттестацию, вы должны были уже разобрать все статьи в этом модуле. |
| ------------------- | ------------------------------------------------------------------------------------------------------- |
| Цели:               | Проверить знания о HTML таблицах и связанными с ними возможностями.                                     |

## Отправная точка

Для того, чтобы начать аттестацию, скопируйте [blank-template.html](https://github.com/mdn/learning-area/blob/master/html/tables/assessment-start/blank-template.html), [minimal-table.css](https://github.com/mdn/learning-area/blob/master/html/tables/assessment-start/minimal-table.css), и [planets-data.txt](https://github.com/mdn/learning-area/blob/master/html/tables/assessment-start/planets-data.txt) в новую директорию на вашем компьютере.

> [!NOTE]
> В качестве альтернативы, вы можете использовать такие сайты, как [JSBin](https://jsbin.com/) или [Glitch](https://glitch.com/), чтобы пройти аттестацию. Вы можете вставлять HTML, CSS и JavaScript в один из этих онлайн редакторов. Если используемый вами онлайн редактор не имеет отдельных JavaScript/CSS панелей, не стесняйтесь вставлять `<script>`/`<style>` элементы в HTML страницу.

## Краткое описание проекта

Вы работаете в школе. В настоящее время ваши ученики изучают планеты солнечной системы, и вы хотите обеспечить их наглядным пособием для поиска фактов и данных о планетах. Таблица HTML была бы идеальным вариантом — вам необходимо взять необработанные данные, которые у вас есть, и превратить их в таблицу, следуя нижеприведённым инструкциям.

Готовая таблица должна выглядеть так:

![](assessment-table.png)

Вы можете также [посмотреть на готовый вариант здесь](https://mdn.github.io/learning-area/html/tables/assessment-finished/planets-data.html) (не смотрите на исходный код — не жульничайте!).

## Шаги для завершения

Следующие шаги описывают что вам нужно сделать, чтобы завершить пример таблицы. Все данные, что вам нужны находятся в файле `planets-data.txt`. Если у вас возникли проблемы с визуализацией данных, посмотрите приведённый выше пример или попробуйте нарисовать диаграмму.

1. Откройте вашу копию `blank-template.html` , и запустите таблицу, предоставив ей внешний контейнер, заголовок и тело таблицы. Вам не нужен нижний колонтитул (footer) для этого примера.
2. Добавьте предоставленную подпись к вашей таблице ("Caption" в конце `planets-data.txt`).
3. Добавьте строку в заголовок таблицы, содержащую все заголовки столбцов.
4. Создайте все строки содержимого внутри тела таблицы, помня, что все заголовки строк должны быть _семантически_.
5. Убедитесь, что весь контент помещён в нужные ячейки - в исходных данных каждая строка данных о планете отображается рядом со связанной с ней планетой.
6. Добавьте атрибуты, чтобы заголовки строк и столбцов были однозначно связаны со строками, столбцами или группами строк, для которых они выступают в качестве заголовков.
7. Добавьте чёрную рамку вокруг столбца, который содержит все заголовки строк с именами планет.

## Подсказки и советы

- Первая ячейка строки заголовка должна быть пустой, и занимать два столбца.
- Заголовки групповых строк (например, _Jovian planets_), которые расположены слева от заголовков строк с именами планет (например, _Saturn_), немного сложно разобрать - необходимо убедиться, что каждый из них охватывает правильное количество строк и столбцов.
- Один из способов связать заголовки с их строками / столбцами намного проще, чем другой.

## Аттестация или дальнейшая помощь

Если вы хотите, чтобы ваша работа была оценена, или вы застряли и хотите обратиться за помощью:

1. Разместите свою работу в онлайн-редакторе, таком как [CodePen](https://codepen.io/), [jsFiddle](https://jsfiddle.net/) или [Glitch](https://glitch.com/).
2. Напишите сообщение с просьбой об оценке и/или помощи в [разделе обучения на форуме MDN Discourse](https://discourse.mozilla.org/c/mdn/learn). Ваш пост должен включать:
   - Описательный заголовок, такой как «Требуется оценка для структурирования данных планеты».
   - Детали того, что вы уже пробовали, и что вы хотели бы, чтобы мы сделали, например, если вы застряли и нуждаетесь в помощи, или хотите оценить свою работу.
   - Ссылка на пример, который вы хотите оценить или в котором вам нужна помощь, в онлайн-редакторе (как упомянуто в шаге 1 выше). Это хорошая практика в решении проблем - очень сложно помочь кому-то с проблемой кода, если вы не видите его код.
   - Ссылка на актуальную задачу или страницу оценки, чтобы мы могли найти вопрос, с которым вам нужно помочь.

{{PreviousMenu("Learn/HTML/Tables/Advanced", "Learn/HTML/Tables")}}
