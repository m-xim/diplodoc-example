::: page-constructor
blocks:
  - type: header-block
    width: xs
    offset: default
    title: Как всё устроено?
    resetPaddings: true
    verticalOffset: l
    description: |-
      Diplodoc — это платформа документации со следущими компонентами:
      * клиентская часть отвечает за отображение документов в браузере на стороне пользователя;
      * серверная часть отвечает за хостинг и выдачу документов клиенту;
      * инструменты создания и преобразования документов из Markdown в статический сайт (Transform & Build).

      Система выполняет основные операции на Node.js и React.
    background:
      image:
        src: https://storage.yandexcloud.net/diplodoc-www-assets/pages/how-to-diplodoc/ddos-how-cover.png
        disableCompress: true
  - type: extended-features-block
    title:
      text: Подход Docs as Сode
    colSizes:
      all: 12
      xl: 3
      md: 4
      sm: 6
    items:
      - title: Markdown
        icon: https://storage.yandexcloud.net/cloud-www-assets/pages/how-to-diplodoc/how-to-diplodoc-01.svg
        text: Документация пишется на языке разметки Markdown, а не в plain text или WYSIWYG-редакторе.
      - title: Хранение в репозитории
        icon: https://storage.yandexcloud.net/cloud-www-assets/pages/how-to-diplodoc/how-to-diplodoc-02.svg
        text: 'Документация хранится в репозитории с остальным кодом. Это может быть GitHub или ваше собственное решение. '
      - title: Налаженный процесс
        icon: https://storage.yandexcloud.net/cloud-www-assets/pages/how-to-diplodoc/how-to-diplodoc-03.svg
        text: Документация собирается в финальный проект при помощи генератора статических сайтов и публикуется автоматически.
      - title: Синхронизация
        icon: https://storage.yandexcloud.net/cloud-www-assets/pages/how-to-diplodoc/how-to-diplodoc-04.svg
        text: Документация пишется и обновляется совместно — точно так же, как и остальной код.
  - type: card-layout-block
    title: Хранение данных
    children:
      - type: layout-item
        content:
          title: Добавление
          text: Исходный код документации хранится в репозитории клиента в формате Markdown.
        media:
          image: https://storage.yandexcloud.net/diplodoc-www-assets/pages/how-to-diplodoc/ddos-how-item-02-01.png
      - type: layout-item
        content:
          title: Преобразование
          text: Преобразованный из Markdown-файлов документационный проект попадает в отдельную директорию S3-совместимого хранилища для каждого клиента.
        media:
          image: https://storage.yandexcloud.net/diplodoc-www-assets/pages/how-to-diplodoc/ddos-how-item-02-02.png
      - type: layout-item
        content:
          title: Доступ
          text: Доступ к S3 регулируется с помощью уникальных ключей.
        media:
          image: https://storage.yandexcloud.net/diplodoc-www-assets/pages/how-to-diplodoc/ddos-how-item-02-03.png
  - type: card-layout-block
    title: Развёртывание
    colSizes:
      all: 12
      xl: 3
      md: 4
      sm: 6
    children:
      - type: layout-item
        content:
          title: Хранение
          text: Документационный проект из S3-совместимого хранилища выкладывается на Diplodoc.com.
        media:
          image: https://storage.yandexcloud.net/diplodoc-www-assets/pages/how-to-diplodoc/ddos-how-item-03-01.png
      - type: layout-item
        content:
          title: Проксирование
          text: Возможно проксирование с сайта клиента на сайт diplodoc.com для бесшовной интеграции.
        media:
          image: https://storage.yandexcloud.net/diplodoc-www-assets/pages/how-to-diplodoc/ddos-how-item-03-02.png
      - type: layout-item
        content:
          title: Поиск
          text: 'Поддержка поиска с помощью Elasticsearch.  '
        media:
          image: https://storage.yandexcloud.net/diplodoc-www-assets/pages/how-to-diplodoc/ddos-how-item-03-03.png
      - type: layout-item
        content:
          title: Локализация
          text: 'Поддержка локализации и кастомизации проекта документации. '
        media:
          image: https://storage.yandexcloud.net/diplodoc-www-assets/pages/how-to-diplodoc/ddos-how-item-03-04.png
  - type: card-layout-block
    title: Полная совместимость
    children:
      - type: background-card
        title: YFM
        text: Диалект Markdown, соответствующий спецификации CommonMark, с поддержкой плагинов и дополнительными возможностями разметки.
        background:
          src: https://storage.yandexcloud.net/diplodoc-www-assets/pages/how-to-diplodoc/ddos-how-card-01.png
          disableCompress: true
        paddingBottom: m
        border: none
      - type: background-card
        title: GitHub
        text: Полная интеграция с системами контроля версий, в первую очередь, с GitHub — одним из основных инструментов разработки.
        background:
          src: https://storage.yandexcloud.net/diplodoc-www-assets/pages/how-to-diplodoc/ddos-how-card-02.png
          disableCompress: true
        paddingBottom: m
        border: none
      - type: background-card
        title: Elasticsearch
        text: Быстрая индексация и поиск на основе Elasticsearch для обеспечения релевантности и точности результатов запросов.
        background:
          src: https://storage.yandexcloud.net/diplodoc-www-assets/pages/how-to-diplodoc/ddos-how-card-03.png
          disableCompress: true
        paddingBottom: m
        border: none
  - type: icons-block
    size: m
    title: Присоединяйтесь к сообществу
    items:
      - src: https://storage.yandexcloud.net/cloud-www-assets/pages/index-diplodoc/github.svg
        text: GitHub
        url: '#'
      - src: https://storage.yandexcloud.net/cloud-www-assets/pages/index-diplodoc/telegram.svg
        text: Telegram
        url: '#'
      - src: https://storage.yandexcloud.net/cloud-www-assets/pages/index-diplodoc/stackoverflow.svg
        text: Stack Overflow
        url: '#'
animated: true
:::
