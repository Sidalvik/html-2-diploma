# Задание на дипломный проект курса «HTML-вёрстка: с нуля до первого макета»

В рамках дипломного проекта вам необходимо сверстать макет сайта, который выглядит следующим образом:
 
 ![](sources/NOEMI_Modern_ru.jpg)

## Требования к дипломному проекту

#### Содержание
- [Кроссбраузерная верстка](#Кроссбраузерная-верстка)
- [Семантическое использование тегов](#Семантическое-использование-тегов)
- [Использование тегов для стилизации элементов](#Использование-тегов-для-стилизации-элементов)
- [Семантические названия атрибутов](#Семантические-названия-атрибутов)
- [Соответствие верстки макету](#Соответствие-верстки-макету)
- [Добавление меньшего или большего количества контента в блоки](#Добавление-меньшего-или-большего-количества-контента-в-блоки)
- [Высота элементов должна рассчитываться по контенту](#Высота-элементов-должна-рассчитываться-по-контенту)
- [Верстка однотипных элементов](#Верстка-однотипных-элементов)
- [Требования к поведению элементов в проекте](#Требования-к-поведению-элементов-в-проекте)
- [Ошибки загрузки изображений](#Ошибки-загрузки-изображений)
- [Верстка текста написанного заглавными буквами](#Верстка-текста-написанного-заглавными-буквами)
- [Верстка декоративных линий у заголовков](#Верстка-декоративных-линий-у-заголовков)
- [Верстка маски для изображений](#Верстка-маски-для-изображений)
- [В HTML не должно быть пустых тегов](#В-HTML-не-должно-быть-пустых-тегов)
- [Верстка отступов](#Верстка-отступов)
- [Верстка иконок](#Верстка-иконок)
- [Верстка скрытого текстового описания у полей ввода](#Верстка-скрытого-текстового-описания-у-полей-ввода)
- [Запрещается использовать CSS методологии](#Запрещается-использовать-CSS-методологии )
- [Запрещается использовать готовые библиотеки](#Запрещается-использовать-готовые-библиотеки)
- [Запрещается использовать CSS препроцессоры или PostCSS](#Запрещается-использовать-CSS-препроцессоры-или-PostCSS)
- [Запрещается использовать autoprefixer](#Запрещается-использовать-autoprefixer)
- [Оформление кода](#Оформление-кода)
- [Реализация дипломного проекта в Codepen](#Реализация-дипломного-проекта-в-Codepen)


### Кроссбраузерная верстка

В рамках проекта сверстанный макет должен корректно отображаться на компьютерах с операционными системами Windows и Mac OS.

Кроме поддержки основных типов операционных систем, также требуется, чтобы верстка корректно работала в следующих браузерах:

- последняя версия Google Chrome;
- последняя версия Mozilla FireFox;
- последняя версия Edge;
- последняя версия Opera;
- последняя версия Safari.

В случае, если у вас нет какого-то устройства, постарайтесь его найти. Тестирование на реальных устройствах является обязательным навыком современного специалиста.

### Семантическое использование тегов

При верстке проекта преимущество отдается тегам, имеющим смысл. К примеру, если сверстать раздел «Новости» следующий образом, это будет являться ошибкой:

```html
<div class="news">
  <h2>Новости</h2>
</div>
```

В этом примере следует использовать тег `section`:

```html
<section class="news">
  <h2>Новости</h2>
</section>
```

### Использование тегов для стилизации элементов

Запрещается использовать теги в целях стилизации элементов. Например, если сверстать жирный текст тегом `b`, то это будет ошибкой.

```html
<b>Текст</b>
```

### Семантические названия атрибутов

Кроме использования семантических тегов, также необходимо давать семантические названия значениям атрибутов. Запрещается использовать транслит.

Пример:

```html
 <header class="shapka"></header>
```

Данный пример является грубой ошибкой. Название класса `shapka` следует заменить на `header`. 

Пример корректного названия:

```html
 <header class="header"></header>
```

При именовании классов можно использовать принятый [список классов](https://github.com/yoksel/common-words).  

### Соответствие верстки макету

Итоговый проект должен быть копией макетов, предоставленных дизайнером. При реализации допускаются следующие отличия:

- толщина шрифта в браузерах и фотошопе;
- межсимвольное расстояние;
- различия в отступах — до 3px.

### Описание отображения страницы 

Дизайнер подготовил макет шириной 1660px, но несмотря на это, вам требуется предусмотреть отображение макета на экранах с шириной  больше, чем 1660px. Для этого дизайнер подготовил следующие требования:

- изображение в шапке должно занимать всю ширину экрана;
- контент в шапке должен быть выровнен по центру;
- блок, содержащий контент в шапке, должен иметь отступы по бокам;
- блок, содержащий основную часть страницы, должен иметь отступы по бокам;
- подвал страницы должен иметь отступы по бокам.

### Добавление меньшего или большего количества контента в блоки

Вам обязательно нужно протестировать блоки с информацией, добавив в них больше или меньше контента, чем представлено в макетах. Блоки не должны сломать соседние блоки, текст при этом должен быть полностью читаемым. 

Вам необходимо предусмотреть следующие случаи:

- добавление 2 пунктов в меню;
- удаление  2, 3, 4 пунктов из меню;
- добавление 2-3 слов в заголовке «Блог о творчестве, спорте, и образе жизни»;
- добавление 2 блоков со статьей;
- удаление всех блоков со статьями, кроме первого; 
- добавление 3 абзацев текста в блоке со статьей;
- теги статьи могут располагаться на  двух строках;
- имя автора статьи может быть длиннее и короче, чем в макете;
- дата статьи может быть длиннее и короче, чем в макете;
- добавление 2 статей в разделе «Новые посты»;
- удаление всех статей, кроме первой, в разделе «Новые посты»;
- удаление любого блока из следующих: блок «Новые посты»,  форма поиска, блок «Рассылка», блока «Теги», блок «Темы»;
- отображение 8 иконок соцсетей;
- отображение 3 иконок соцсетей.

### Высота элементов должна рассчитываться по контенту

При верстке элементов вам не нужно фиксировать их высоту, высота должна зависеть от контента внутри элемента. Это необходимо для осуществления пункта [Добавление меньшего или большего количества контента в блоки](#Добавление-меньшего-или-большего-количества-контента-в-блоки). 

Разрешается фиксировать высоту для декоративных элементов: черта под заголовками, иконки, кнопки в форме поиска, поля ввода в формах.

Также при верстке элементов вам необходимо следить за тем, чтобы у элементов свойство `height` не равнялась 0, а все также зависело от контента.

### Верстка однотипных элементов

При работе с макетом вы можете столкнуться с ситуацией когда у однотипных элементов  отличается ширина (или другое свойство) на несколько пикселей. Например, ширина элементов статей в разделе «Новые посты». Визуально они отличаются. 

Это сделано для того, чтобы посмотреть, как будет отображаться разный текст. В вашей вёрстке ширина у этих элементов должна быть одинаковой. Вы можете выбрать самостоятельно один из размеров из макета и задать его для всех однотипных элементов. Не нужно подгонять каждый элемент под размеры макета.

### Требования к поведению элементов в проекте

Вы должны предусмотреть следующие сценария поведения элементов:

- все пункты в меню должны быть ссылками;
- все заголовки статей должны быть ссылками;
- все формы на странице должны отправлять данные;
- все формы на странице должны проверять корректность введенных данных;
- все теги на странице должны быть ссылками;
- в блоке «Темы» каждое название категории должно быть ссылкой;
- в блоке «Темы» количество статей в категории должен быть текстом;
- соц. иконки должны быть ссылками;
- копирайт на странице должен быть ссылкой.

Для всех ссылок на странице используйте атрибут `href` со значением `#0`.


### Ошибки загрузки изображений

При верстке изображений вам нужно предусмотреть ситуацию, когда по какой-либо причине они не загрузятся.

- В случае контентных изображений верстка не должна сломаться, а вместо изображения должен отображаться альтернативный текст, из которого станет понятно, что было изображено на картинке.
- Для декоративных изображений вам необходимо подобрать подложки для текста, чтобы текст был читаемым в любой ситуации.

### Верстка текста написанного заглавными  буквами

Заглавное отображение текста должно быть реализовано с использованием CSS. Запрещается писать текст только заглавными в HTML. Пример ошибки:

```html
    <h3>ЭТО ЗАГОЛОВОК</h3>
```

### Верстка декоративных линий у заголовков

Декоративное подчеркивание у заголовков «Новые посты», «Рассылка», «Теги» и т.п. вам нужно реализовать через псевдоэлементы.  

### Верстка маски для изображений

Маску для изображений вам нужно реализовать через псевдоэлементы.

### В HTML не должно быть пустых тегов

В HTML у вас не должно быть тегов, у которых нет контента.

### Верстка отступов

Вам требуется внимательно реализовывать отступы. Внешние отступы задаются между соседними элементами, а внутренние между родителем и дочерним элементом. Несоблюдение этого правила является ошибкой. 

### Верстка иконок

Все иконки в проекте должны иметь скрытое текстовое описание. Для скрытия текста используйте следующий код:

```css
.visually-hidden {
  width: 1px;
  height: 1px;
  clip: rect(1px, 1px, 1px, 1px);
  position: absolute;
} 
```

Этот фрагмент кода используется в домашнем задании, в котором вы верстали кастомный чекбокс. 


### Верстка скрытого текстового описания у полей ввода

Визуальное текстовое описание полей ввода не предусмотрено дизайнером. Поэтому вам самостоятельно нужно его придумать и скрыть, используя следующий код:

```css
.visually-hidden {
  width: 1px;
  height: 1px;
  clip: rect(1px, 1px, 1px, 1px);
  position: absolute;
} 
```

Текстовое описание должно быть понятным и объяснять, какие данные нужно вводить в поля. Его нужно задать и для кнопки поиска, поскольку на кнопке нет текста.

### Запрещается использовать CSS методологии 

В рамках курса мы не рассматриваем CSS методологии такие как: БЭМ, OOCSS, SMACSS и другие. Поэтому в дипломе запрещается их использовать. 

### Запрещается использовать готовые библиотеки

В рамках дипломного проекта запрещается использовать готовые библиотеки (например, normalize.css, reset.css, bootstrap и другие). Весь код вы должны написать самостоятельно.

### Запрещается использовать CSS препроцессоры или PostCSS

В рамках курса  мы не рассматриваем способы организации кода с использованием CSS препроцессоров и PostCSS. Поэтому в дипломе вам запрещается их использовать.

### Запрещается использовать autoprefixer

Для реализации кроссбраузерной верстки дипломного проекта вам не потребуется autoprefixer, поэтому его использование запрещено.

### Оформление кода

Дипломный проект обязательно должен соответствовать принятому стилю кода для [HTML](https://github.com/netology-code/codestyle/tree/master/html) и [CSS](https://github.com/netology-code/codestyle/tree/master/css). В случае ошибок в оформлении проект не может быть принят и будет отправлен на доработку.

### Порядок следования CSS-правил 

При реализации проекта порядок CSS-правил должен совпадать с порядком следования элементов в HTML. Например, есть HTML

```html
    <header class="header">
      <h1 class="header-title">Заголовок</h1>
    </header>
    <main class="main">
      <section class="section">
        <h2 class="section-title">Новости</h2>
      </section>
    </main>
```

Для стилизации структуры нужно использовать следующий порядок CSS-правил

```css
    .header { 
      padding: 10px;
    }
    
    .header-title {
      font-size: 20px;
    }
    
    .main {
      margin-left: auto;
      margin-right: auto;
    }
    
    .section {
      background-color: #eeeeee;
    }
    
    .section-title {
      font-size: 18px;
    }
```

### Реализация дипломного проекта в Codepen

Дипломный проект должен быть реализован на сайте Codepen. Вам не нужно создавать основной каркас страницы. Во вкладке HTML создайте сразу разметку страницы без элемента `body`. Для подключения декоративных элементов, изображений и шрифтов проекта используйте ссылки из файла [Ресурсы проекта](https://github.com/netology-code/html-2-diploma/blob/master/sources/README.md)



### Как правильно задавать вопросы дипломному руководителю?

**Что следует делать, чтобы все получилось:**

* Попробовать найти ответ сначала самому в интернете. Ведь, именно это скилл поиска ответов пригодится тебе на первой работе. И только после этого спрашивать дипломного руководителя
* В одном вопросе должна быть заложена одна проблема 
* По возможности, прикреплять к вопросу скриншоты и стрелочкой показывать где не получается. Программу для этого можно скачать здесь https://app.prntscr.com/ru/
* По возможности, задавать вопросы в комментариях к коду. 
* Начинать работу над дипломом как можно раньше! Чтобы было больше времени на правки. 
* Делать диплом по-частям, а не все сразу. Иначе, есть шанс, что нужно будет все переделывать :)  

**Что следует делать, чтобы ничего не получилось:**

* Писать вопросы вида “Ничего не работает. Не запускается. Всё сломалось.”
* Откладывать диплом на потом. 
* Ждать ответ на свой вопрос моментально. Дипломные руководители - работающие разработчики, которые занимаются, кроме преподавания, своими проектами. Их время ограничено, поэтому постарайтесь задавать правильные вопросы, чтобы получать быстрые ответы! 
