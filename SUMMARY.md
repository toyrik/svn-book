# Summary

* [Предисловие](foreword.md)
* [Об этой книге](preface.md)
  * [Для кого написана эта книга?](preface-audience.md)
  * [Как читать эту книгу?](preface-howread.md)
  * [Соглашения, принятые в книге](preface-conventions.md)
  * [Структура книги](preface-organisation.md)
  * [Эта книга распространяется свободно](preface-free.md)
  * [Благодарности](preface-acks.md)
  * [Что такое Subversion?](intro-whatis.md)
* [1. Фундаментальные понятия]()
  * [Хранилище]()
  * [Модели версионирования]()
    * [Проблема разделения файлов]()
    * [Модель Блокирование-Изменение-Разблокирование]()
    * [Модель Копирование-Изменение-Слияние]()
  * [Subversion в действии]()
    * [URL хранилища в Subversion]()
    * [Рабочие копии]()
    * [Правки]()
    * [Как рабочие копии отслеживают хранилище]()
    * [Смешивание правок в рабочих копиях]()
    * [Обновления и фиксации отделены друг от друга]()
      * [Смешивание правок — это нормально]()
      * [Смешивание правок — это полезно]()
      * [Смешивание правок имеет ограничения]()
  * [Подводя итоги* Экскурсия по Subversion]()
  * [Читайте справку!]()
  * [Импорт]()
  * [Путешествие во времени вместе с Subversion]()
  * [Создание рабочей копии]()
  * [Простейший рабочий цикл]()
    * [Обновление рабочей копии]()
    * [Внесение изменений в рабочую копию]()
    * [Анализ изменений]()
      * [svn status]()
      * [svn diff]()
      * [svn revert]()
    * [Разрешение конфликтов (при слиянии с чужими зменениями)]()
      * [Слияние конфликтов вручную]()
      * [Копирование файла поверх вашего рабочего файла]()
      * [Использование svn revert]()
    * [Фиксация изменений]()
  * [Анализ истории]()
    * [svn log]()
    * [svn diff]()
      * [Анализ локальных изменений]()
      * [Сравнение рабочей копии с хранилищем]()
      * [Сравнение хранилища с хранилищем]()
    * [svn cat]()
    * [svn list]()
    * [Заключительное слово об истории]()
    Другие полезные команды
        svn cleanup
        svn import
    Подводя итоги
Профессиональное использование Subversion
    Способы обозначения правок
        Ключевые слова правок
        Даты правок
    Свойства
        Зачем нужны свойства?
        Использование свойств
        Свойства и рабочий цикл Subversion
        Автоматическая установка свойств
    Переносимость файлов
        Тип содержимого файла
        Исполнимость файла
        Символы конца строки
    Пропуск неверсионированных элементов
    Подстановка ключевых слов
    Locking
        Creating locks
        Discovering locks
        Breaking and stealing locks
        Lock Communication
    Внешние зависимости
    Стержневые и оперативные правки
Ветвление и слияние
    Что такое ветка?
    Использование веток
        Создание ветки
        Работа с веткой
        Ключевые идеи, стоящие за ветками
    Копирование изменений между ветками
        Копирование отдельных изменений
        Ключевые идеи, стоящие за слиянием
        Как правильнее всего использовать слияние
            Ручной контроль слияния
            Предварительный просмотр результатов слияния
            Конфликты при слиянии
            Учитывать или игнорировать происхождение
    Типовые примеры
        Полное объединение двух веток
        Отмена изменений
        Восстановление удаленных элементов
        Типовые приемы использования веток
            Ветки релизов
            Функциональные ветки
    Переключение рабочей копии
    Метки
        Создание простой метки
        Создание комплексной метки
    Поддержка веток
        Структура хранилища
        Продолжительность жизни информации
    Vendor branches
        General Vendor Branch Management Procedure
        svn_load_dirs.pl
    Подводя итоги
Администрирование хранилища
    Repository Basics
        Understanding Transactions and Revisions
        Unversioned Properties
        Repository Data Stores
            Berkeley DB
            FSFS
    Repository Creation and Configuration
        Hook Scripts
        Berkeley DB Configuration
    Repository Maintenance
        An Administrator's Toolkit
            svnlook
            svnadmin
            svndumpfilter
            Berkeley DB Utilities
        Repository Cleanup
        Managing Disk Space
        Repository Recovery
        Migrating a Repository
        Repository Backup
    Adding Projects
        Choosing a Repository Layout
        Creating the Layout, and Importing Initial Data
    Summary
Настройка сервера
    Обзор
        Http-сервер Apache
        Сервер svnserve
        svnserve через SSH
        Выбор лучшей конфигурации сервера
    Сетевая модель
        Запросы и отклики
        Кэширование клиентской идентификационной информации
    Собственный сервер svnserve
        Запуск Сервера
        Встроенная аутентификация и авторизация
            Создание файла пользователей и область хранилища
            Установка контроля доступа
        SSH идентификация и авторизация
        Трюки конфигурирования SSH
            Начальная настройка
            Controlling the invoked command
    httpd, the Apache HTTP server
        Prerequisites
        Basic Apache Configuration
        Authentication Options
            Basic HTTP Authentication
            SSL Certificate Management
        Authorization Options

            Blanket Access Control
            Per-Directory Access Control
            Disabling Path-based Checks

        Extra Goodies

            Repository Browsing
            Other Features

    Path-Based Authorization
    Supporting Multiple Repository Access Methods

Профессиональная настройка Subversion

    Параметры времени выполнения

        Структура области конфигурации
        Конфигурация и реестр Windows
        Параметры конфигурации

            Servers
            Config

    Localization

        Understanding locales
        Subversion's use of locales

    Using External Differencing Tools

        External diff
        External diff3

Информация для разработчиков

    Layered Library Design

        Repository Layer
        Repository Access Layer

            RA-DAV (Repository Access Using HTTP/DAV)
            RA-SVN (Custom Protocol Repository Access)
            RA-Local (Direct Repository Access)
            Your RA Library Here

        Client Layer

    Using the APIs

        The Apache Portable Runtime Library
        URL and Path Requirements
        Using Languages Other than C and C++

    Inside the Working Copy Administration Area

        The Entries File
        Pristine Copies and Property Files

    WebDAV

9. Полное справочное руководство по Subversion

    Клиент командной строки Subversion: svn

        Параметры командной строкиsvn
        Подкоманды svn

            svn add
            svn blame
            svn cat
            svn checkout
            svn cleanup
            svn commit
            svn copy
            svn delete
            svn diff
            svn export
            svn help
            svn import
            svn info
            svn list
            svn lock
            svn log
            svn merge
            svn mkdir
            svn move
            svn propdel
            svn propedit
            svn propget
            svn proplist
            svn propset
            svn resolved
            svn revert
            svn status
            svn switch
            svn unlock
            svn update

    svnadmin

        svnadmin Switches
        svnadmin Subcommands

            svnadmin create
            svnadmin deltify
            svnadmin dump
            svnadmin help
            svnadmin hotcopy
            svnadmin list-dblogs
            svnadmin list-unused-dblogs
            svnadmin load
            svnadmin lslocks
            svnadmin lstxns
            svnadmin recover
            svnadmin rmlocks
            svnadmin rmtxns
            svnadmin setlog
            svnadmin verify

    svnlook

        svnlook Switches
        svnlook

            svnlook author
            svnlook cat
            svnlook changed
            svnlook date
            svnlook diff
            svnlook dirs-changed
            svnlook help
            svnlook history
            svnlook info
            svnlook lock
            svnlook log
            svnlook propget
            svnlook proplist
            svnlook tree
            svnlook uuid
            svnlook youngest

    svnserve

        svnserve Switches

    svnversion

        svnversion

    mod_dav_svn

        mod_dav_svn Configuration Directives

    Свойства Subversion

        Свойства Subversion

A. Быстрый старт в Subversion

    Установка Subversion
    Быстрый старт в Subversion

B. Subversion для пользователей CVS

    Revision Numbers Are Different Now
    Directory Versions
    More Disconnected Operations
    Distinction Between Status and Update

        Status
        Update

    Branches and Tags
    Metadata Properties
    Conflict Resolution
    Binary Files and Translation
    Versioned Modules
    Authentication
    Converting a Repository from CVS to Subversion

C. WebDAV и автоматическое управление версиями

    Basic WebDAV Concepts

        Original WebDAV
        DeltaV Extensions

    Subversion and DeltaV
    Autoversioning
    Client Interoperability

        Standalone WebDAV applications

            Microsoft Office, Dreamweaver, Photoshop
            Cadaver, DAV Explorer

        File-explorer WebDAV extensions

            Microsoft Web Folders
            Nautilus, Konqueror

        WebDAV filesystem implementation

            WebDrive, NetDrive
            Mac OS X
            Linux davfs2

D. Инструменты от сторонних разработчиков
E. Copyright
Предметный указатель
Русский глоссарий

Список иллюстраций

1. Архитектура Subversion
1.1. Типичная клиент/серверная система
1.2. Проблема потери изменений
1.3. Модель блокирование-изменение-разблокирование
1.4. Модель копирование-изменение-слияние
1.5. Модель копирование-изменение-слияние (продолжение)
1.6. Файловая система хранилища
1.7. Хранилище
4.1. Ветки разработки
4.2. Начальная структура хранилища
4.3. Хранилище, содержащее новую копию
4.4. История ветвления для одного файла
8.1. Files and directories in two dimensions
8.2. Versioning time—the third dimension!

Список таблиц

1.1. URL для доступа к хранилищу.
5.1. Repository Data Store Comparison
6.1. Сравнение серверов
8.1. A Brief Inventory of the Subversion Libraries
C.1. Common WebDAV Clients

Список примеров

5.1. txn-info.sh (Reporting Outstanding Transactions)
6.1. A sample configuration for anonymous access.
6.2. A sample configuration for authenticated access.
6.3. A sample configuration for mixed authenticated/anonymous access.
6.4. Disabling path checks altogether
7.1. Пример указания параметров в (.reg) файле реестра.
7.2. diffwrap.sh
7.3. diffwrap.bat
7.4. diff3wrap.sh
7.5. diff3wrap.bat
8.1. Using the Repository Layer
8.2. Using the Repository Layer with Python
8.3. A Python Status Crawler
8.4. Contents of a Typical .svn/entries File
