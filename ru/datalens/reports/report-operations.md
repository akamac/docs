# Работа с отчетом


{% include [business-note](../../_includes/datalens/datalens-functionality-available-business-note.md) %}


В этом разделе вы узнаете, как работать с отчетом:

* [{#T}](#create-report)
* [{#T}](#report-pages)
* [{#T}](#report-widget-settings)
* [{#T}](#report-settings)
* [{#T}](#page-settings)
* [{#T}](#report-export)

## Создать отчет {#create-report}



Отчет можно создать одним из способов:

{% list tabs %}

- Воркбук

  1. Перейдите на [страницу коллекций и воркбуков]({{ link-datalens-main }}/collections).
  1. Откройте [воркбук](../workbooks-collections/index.md), в котором хотите создать отчет.
  1. В правом верхнем углу нажмите кнопку **Создать** и выберите **Отчёт**.
  1. [Добавьте страницы](#report-pages) в отчет.
  1. [Добавьте](#add-widget) на страницы необходимые [виджеты](../dashboard/widget.md).
  1. [Настройте отчет](#report-settings) и его отдельные [страницы](#page-settings).
  1. В правом верхнем углу экрана нажмите кнопку **Сохранить**.
  1. В открывшемся окне введите название отчета и нажмите кнопку **Создать**.

- Панель навигации

  1. Перейдите на [главную страницу]({{ link-datalens-main }}) {{ datalens-short-name }}.
  1. На панели слева выберите ![image](../../_assets/console-icons/display-pulse.svg) **Отчёты** и нажмите кнопку **Создать отчёт**.
  1. [Добавьте страницы](#report-pages) в отчет.
  1. [Добавьте](#add-widget) на страницы необходимые [виджеты](../dashboard/widget.md).
  1. [Настройте отчет](#report-settings) и его отдельные [страницы](#page-settings).
  1. В правом верхнем углу экрана нажмите кнопку **Сохранить**.
  1. В открывшемся окне введите название отчета и нажмите кнопку **Создать**.

{% endlist %}





Созданный отчет можно [экспортировать](#report-export).

## Добавить, переместить или удалить страницы {#report-pages}

В отчет можно добавить несколько страниц, изменить их порядок или удалить:

* Чтобы добавить страницу, внизу слева нажмите кнопку ![image](../../_assets/console-icons/plus.svg) **Добавить страницу**.
* Чтобы дублировать страницу, в области предпросмотра нажмите значок ![image](../../_assets/console-icons/ellipsis.svg) у страницы и выберите ![icon](../../_assets/console-icons/copy.svg) **Дублировать**.
* Чтобы изменить порядок страниц, перетаскивайте их на новое место с помощью мыши.
* Чтобы удалить страницу, в области предпросмотра нажмите значок ![image](../../_assets/console-icons/ellipsis.svg) у страницы и выберите ![icon](../../_assets/console-icons/trash-bin.svg) **Удалить**.

## Настроить виджеты {#report-widget-settings}

Вы можете добавить, скопировать или удалить виджеты в отчете. При наложении виджетов друг на друга можно переместить их на передний или задний план.

### Добавить виджет {#add-widget}

1. Выберите страницу отчета, на которую хотите добавить виджет.
1. Выберите виджет: [Чарт](../concepts/chart/index.md), [Текст](../dashboard/widget.md#text), [Заголовок](../dashboard/widget.md#title) или Изображение. Чтобы сразу разместить виджет в нужном месте на странице, перетащите его с зажатой левой кнопкой мыши.
1. Настройте виджет:

   {% list tabs %}

   - Чарт

     * **Название** — имя виджета. Если опция **Показывать** включена (по умолчанию), название отображается в верхней части виджета.
     * **Чарт** — выберите чарт из списка объектов или укажите ссылку на нужный чарт.
     * (опционально) **Описание** — текст, который отображается в нижней части виджета.
     * (опционально) В разделе **Параметры** введите список [параметров чарта](../dashboard/dashboard_parameters.md#params-chart) и их значения по умолчанию. Если значения по умолчанию не заданы, в отчете отобразится ошибка.
     * (опционально) Задайте фон.

   - Текст

     * Введите текст ссылки, поясняющей надписи и т.д. Виджет поддерживает язык разметки [Markdown](../dashboard/markdown.md).

       {% note warning %}

       Если вставляете в виджет изображение, размещенное в хранилище {{ objstorage-full-name }}, задайте настройки [CORS](../../storage/operations/buckets/cors.md) для бакета с изображением:

       {% include [datalens-cors-settings-note](../../_includes/datalens/datalens-cors-settings-note.md) %}

       {% endnote %}

     * (опционально) Задайте фон.

   - Заголовок

     * Введите текст заголовка.
     * Выберите размер.
     * (опционально) Задайте фон.

   - Изображение

     * Добавьте ссылку на [изображение](../dashboard/markdown.md#image), размещенное в хранилище [{{ objstorage-full-name }}](../../storage/quickstart.md).

       {% note warning %}

       В {{ objstorage-full-name }} необходимо задать настройки [CORS](../../storage/operations/buckets/cors.md) для бакета с изображением:

       {% include [datalens-cors-settings-note](../../_includes/datalens/datalens-cors-settings-note.md) %}

       {% endnote %}  

     * (опционально) Укажите альтернативный текст, который будет отображаться, если не удастся загрузить изображение.
     * (опционально) Отключите опцию сохранения соотношения сторон при изменении размеров виджета. По умолчанию опция включена.
     * (опционально) Задайте фон.

   {% endlist %}

1. Нажмите кнопку **Добавить**.
1. Измените размер виджета и переместите его в удобное место на странице.
1. В правом верхнем углу нажмите кнопку **Сохранить**.

Вы можете скопировать и вставить на страницу уже созданный виджет:


* с любой страницы текущего отчета;
* со страницы другого отчета в том же воркбуке;
* из любого дашборда в том же воркбуке.



Чтобы вставить на страницу скопированный виджет:

1. Нажмите значок ![image](../../_assets/console-icons/ellipsis.svg) у виджета, который хотите скопировать, и выберите ![icon](../../_assets/console-icons/copy.svg) **Копировать**. Скопировать виджет с дашборда можно в режиме редактирования.
1. Выберите страницу отчета, на которую хотите вставить виджет.
1. Сверху на панели виджетов нажмите ![icon](../../_assets/console-icons/copy-plus.svg) **Вставка**.
1. Измените размер виджета и переместите его в удобное место на странице.
1. В правом верхнем углу нажмите кнопку **Сохранить**.

### Удалить виджет {#delete-widget}

1. Выберите страницу отчета, на которой расположен виджет.
1. Нажмите значок ![image](../../_assets/console-icons/ellipsis.svg) у виджета и выберите ![icon](../../_assets/console-icons/trash-bin.svg) **Удалить**.
1. В правом верхнем углу нажмите кнопку **Сохранить**.

### Переместить виджет на передний или задний план {#move-widget-front-or-back}

Виджеты на странице располагаются слоями, которые накладываются друг на друга. Порядок виджетов на странице можно задать вручную:

1. Выберите страницу отчета, на которой расположен виджет.
1. Нажмите значок ![image](../../_assets/console-icons/ellipsis.svg) у виджета и выберите:

   * ![icon](../../_assets/console-icons/arrow-up-to-line.svg) **На передний план** — чтобы переместить виджет на передний план.
   * ![icon](../../_assets/console-icons/arrow-down-to-line.svg) **На задний план** — чтобы переместить виджет на задний план.

1. В правом верхнем углу нажмите кнопку **Сохранить**.

Когда вы взаимодействуете с виджетом — выделяете его или перемещаете по странице — он автоматически накладывается поверх других виджетов. После того как вы перестанете с ним взаимодействовать, он вернется на свой слой.

## Настроить отчет {#report-settings}

Настройки отчета применяются ко всем его страницам:

1. Вверху справа нажмите ![icon](../../_assets/console-icons/gear.svg) **Настройки отчёта**.
1. Настройте внешний вид:

   * **Тема** — выберите тему оформления страницы: ![icon](../../_assets/console-icons/sun.svg) светлую или ![icon](../../_assets/console-icons/moon.svg) темную.
   * **Цвет фона** — задайте цвет в шестнадцатеричном формате или выберите цвет из цветовой палитры.
   * **Формат** — выберите формат: `A4` или `A3`.
   * **Ориентация** — выберите ориентацию: `Альбомная` или `Портретная`.

1. Задайте настройки колонтитула:

   * **Стандартный колонтитул {{ datalens-short-name }}** — добавляет колонтитул: `Построено в {{ datalens-full-name }}`.
   * **Колонтитул на первой странице** — повторяет колонтитул на первой странице. По умолчанию на первой странице колонтитул не отображается.
   * **Нумерация страниц** — добавляет в колонтитул номер страницы.

## Настроить страницы {#page-settings}

Для каждой страницы можно задать индивидуальные настройки, которые отличаются от общих настроек отчета. По умолчанию для страницы действуют [настройки отчета](#report-settings).

{% note info %}

Настройки страницы обладают большим приоритетом, чем такие же настройки отчета. Если в настройках страницы соответствующие настройки имеют другие значения, будут применены они.

{% endnote %}

1. Выберите страницу отчета, которую нужно настроить.
1. Вверху справа нажмите ![icon](../../_assets/console-icons/gear.svg) **Настройки страницы** и включите нужные настройки:

   * **Тема** — тема оформления страницы: ![icon](../../_assets/console-icons/sun.svg) светлая или ![icon](../../_assets/console-icons/moon.svg) темная.
   * **Цвет фона** — задайте цвет в шестнадцатеричном формате или выберите цвет из цветовой палитры.
   * **Формат** — формат страницы: `A4` или `A3`.
   * **Ориентация** — ориентация страницы: `Альбомная` или `Портретная`.

1. В правом верхнем углу нажмите кнопку **Сохранить**.

## Экспортировать отчет {#report-export}

Чтобы экспортировать отчет, нажмите кнопку **Экспорт**. Отчет экспортируется в файл формата `.pdf`.
