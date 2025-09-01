# Перечень терминов

**Таблица 1**. Термины, используемые в руководстве **Kodify**.

| Термин | Описание | 
|-------|-----|
|Генерация кода| Автоматическое создание программного кода специальным приложением (генератором кода) по заданным условиям. |
|Искусственный интеллект| Область компьютерных наук, занимающаяся созданием вычислительных систем, способных выполнять задачи, требующие человеческого интеллекта, такие как восприятие, рассуждение, обучение и решение проблем. |
|Машинное обучение| Раздел искусственного интеллекта, в котором вычислительные системы обучаются выполнять задачи, анализируя и обобщая данные. Обучение происходит без явного программирования специфических инструкций. |
|Токен| Минимальная единица текста, например, слово или символ. Применяется в обработке естественного языка для анализа и генерации текста. |
|Unit-тестирование | Проверка корректности работы отдельных модулей исходного кода программы (функций, методов, классов). |

# Перечень сокращений

**Таблица 2**. Сокращения в руководстве **Kodify**.

| Сокращение | Описание | 
|-------|-----|
|ПО| Программное обеспечение |
|AI (Artificial Intelligence)| Интеллект, демонстрируемый машинами, в частности компьютерными системами. |
|IDE (Integrated Development Environment)| Программа, в которой разработчики пишут, проверяют, тестируют и запускают код, а также ведут большие проекты. |
|JSON (JavaScript Object Notation)| Текстовый формат обмена данными, который используется для хранения и передачи структурированной информации между системами и приложениями. |
|LLM (Large Language Model)| Генеративная нейронная сеть архитектуры трансформер с миллиардами параметров, обученная на обширных текстовых корпусах для понимания и генерации человекоподобного текста. |
|UI (User Interface)| Пользовательский интерфейс. |


# Введение

Настоящий документ представляет собой руководство пользователя (далее — руководство) системы Kodify.

Руководство описывает:
- общее определение системы;
- функции системы;
- настройку и установку плагина в среде Visual Studio Code;
- настройку и установку плагина в среде JetBrains;
- работу с плагином.

## Краткое описание возможностей

Kodify от MWS AI — AI-ассистент разработчика. Этот инструмент использует искусственный интеллект для автоматизации рутинных процессов и помощи разработчикам в выполнении различных задач при написании программного кода.

Функции Kodify:

- Автопродление кода с помощью LLM, которая на основе уже написанного пользователем кода генерирует завершение строки.
- Документирование кода.
- Поиск и исправление ошибок в коде.
- Оптимизация кода.
- Формирование Unit-тестов для кода пользователя.
- Объяснение кода.
- Создание файлов, написание кода, поиск контента и т.д. в режиме "Agent".

## Уровень подготовки пользователей

Пользователи Системы должны:

- обладать базовыми навыками работы в IDE в средах Visual Studio Code или JetBrains; 
- знать один из популярных языков программирования (например, Python, C#, Java, Go, JavaScript).

## Перечень эксплуатационной документации, с которой необходимо ознакомиться пользователю

Для работы в Системе, пользователь должен ознакомиться с настоящим руководством.

# Назначение и условия применения

Система предназначена для облегчения процесса разработки, предоставляя инструменты для генерации кода, улучшения его качества и автоматизации рутинных задач. Kodify поддерживает различные языки программирования (например, Python, C#, Java, Go, JavaScript) и интеграции с популярными инструментами разработки.

Kodify представляет собой LLM и плагин, встраиваемый в IDE. Взаимодействие пользователя с LLM Kodify осуществляется через пользовательский интерфейс (UI) в виде плагина. Плагин содержит набор функций для упрощения и ускорения процесса написания кода за счёт обращения к LLM. Плагин доступен для Visual Studio Code и JetBrains IDE.

# Подготовка к работе

## Установка плагина в среде Visual Studio Code

> Поддерживаются среды разработки Visual Studio Code и IntelliJ IDEA.

1. Скачайте последнюю версию плагина Kodify для Visual Studio Code. Ссылку для скачивания предоставит сотрудник MWS AI.
2. Откройте Visual Studio Code и перейдите в раздел **"Extensions"** на левой панели инструментов.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/extensions_new.png)
   
3. Откройте диалоговое меню, нажав кнопку "…" и выберите пункт **"Install from VSIX…"**.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/install-from-vsix_new.png)
   
4. В открывшемся окне укажите скачанный файл плагина и нажмите **Install**.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/install-from-vsix-window.png)


## Установка плагина в среде JetBrains

1. Скачайте последнюю версию плагина Kodify для JetBrains. Ссылку для скачивания предоставит сотрудник MWS AI.
2. Запустите IDE и перейдите в настройки.
3. Выберите пункт "Plugins", чтобы перейти к настройке плагинов.
   
    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/pycharm_plugins_new.png)

  
4. Нажмите на шестеренку в правом верхнем углу и выберите **"Install Plugin from Disk…"**.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/install-plugin-from-disk_new.png)
   
5. Выберите скачанный файл плагина в диалоговом окне и нажмите **OK**.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/choose-plugin-file.png)


## Настройка плагина в средах Visual Studio Code и JetBrains

1. Откройте в IDE любой файл.
2. Откройте боковую панель "Kodify", используя следующую комбинацию клавиш:
  - в Visual Studio Code - **"CTRL + L"** (**"CMD + L"** на Mac);
  - в JetBrains - **"CTRL+ J"** (**"CMD + J"** на Mac).

    
   На следующем скриншоте показана боковая панель "Kodify" в Visual Studio Code.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/vscode-kodify-panel_new.png)
    
        
   Боковая панель "Kodify" в JetBrains выглядит следующим образом:    
    
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/jetbrains-kodify-panel_new.png)
    
3. Откройте конфигурационный файл *config.json*.

   На боковой панели откройте меню "Kodify" и нажмите на кнопку "шестеренка".
 
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/vscode-open-settings-button_new.png)

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/jetbrains-kodify-config-button_new.png)
  

4. Заполните конфигурационный файл *config.json*.

   Если вы планируете обращаться к Kodify в контуре MWS AI, то в конфигурационном файле для плагина вам необходимо указать **baseUrl** (адрес сервера, к которому вы будете обращаться) и **токен**, который будет использоваться плагином при отправке API-запросов к серверу. Для получения **baseUrl** и **токена** обратитесь к сотруднику MWS AI.

   **baseUrl** и **токен** требуется указать трижды:
  - в разделе **"models"**  —  поля **"apiBase"** и **"apiKey"**;
  - в разделе **"tabAutocompleteModel"**  —  поля **"apiBase"** и **"apiKey"**;
  - в разделе **"embeddingsProvider"**  —  поля **"apiBase"** и **"apiKey"**.

    Если в контуре вашей компании развёрнут отдельный экземпляр Kodify, то помимо **baseUrl** и **токена** вам потребуется заполнить в конфигурационном файле поле **"model"** (id модели) в следующих разделах:
  - в разделе **"models"**;
  - в разделе **"tabAutocompleteModel"**;
  - в разделе **"embeddingsProvider"**.

5. Сохраните настройки файла *config.json* в IDE. Для этого нажмите комбинацию клавиш **"Ctrl+S"** или выберите пункт меню IDE: **File -> Save** (в Visual Studio Code) и **File -> Save All** (в JetBrains).


# Работа с плагином 

> Плагин настроен и готов к работе. Сервис подключится автоматически (при необходимости перезагрузите IDE). 

## Автоматическое дополнение кода

Функция автодополнение кода предлагает вероятный вариант продолжения кода по мере его ввода пользователем в редакторе кода IDE.

1. Откройте любой файл с Python-кодом или кодом на другом языке программирования.
2. Поставьте курсор, например, после **"for i in range(len(x)):"** (смотрите скриншот ниже) и нажмите **ENTER**. Kodify предложит вариант дополнения кода.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/autocompletion-code-suggestion_new.png)
   
3. Нажмите **TAB**, чтобы принять предложенное дополнение кода.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/autocompletion-code-applied_new.png)     

4. Если требуется продолжить автодополнение, нажмите **ENTER** еще раз и повторите шаг 3.

> Если возникли проблемы при установке или настройке, пожалуйста, свяжитесь с нами удобным способом, и мы обязательно поможем.

## Функция общения с Kodify через чат

Kodify помогает разработчикам получить справочную информацию о выделенном коде, не покидая IDE.

1. Откройте файл с кодом и выделите нужную часть кода. Плагин предложит нажать комбинацию клавиш. Для вызова функции "Chat" нажмите:
- в Visual Studio Code — **"Ctrl+L"** для Windows или **"CMD + L"** для Mac;
- в JetBrains — **"Ctrl+J"** для Windows или **"CMD + J"** для Mac.

  ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/vscode-select-code_new.png)     
  
2. В открывшемся окне вы увидите добавленный код, выделенный в редакторе кода. Введите знак "/" в текстовое поле ввода. Появятся доступные варианты:
  
  ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/plugin-functions_new.png)   

- **/test**  — генерирует Unit-test к выделенной части кода;
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-test.png)   

- **/docs** — добавляет docstring к выделенной части кода;
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-docs.png)  

- **/fix** — ищет и исправляет ошибки в выделенной части кода;
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-fix.png)  
- **/explain (rus)**  — объясняет, что делает код на русском языке.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-explain-rus.png) 

   Также, вместо использования одного из предустановленных вариантов, вы можете самостоятельно описать те действия, которые Kodify должен произвести с выделенной частью кода.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-custom-request.png) 

3. Выберите нужный вариант или опишите собственный и нажмите кнопку отправки или **ENTER**.
  
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-send-request_new.png)   

   Вы можете отправить в Kodify контекст в запросе, нажав "@" на панели.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-attach-content.png)  
 
   Можно прикрепить контекст из:
- **Files** — позволяет выбрать файл.
- **Git Diff** — позволяет сослаться на текущий git diff.
- **Folder** — позволяет выбрать папку.
- **Codebase** — Kodify автоматически найдет релевантные файлы.
- **Rules** —  это пользовательские правила в виде Markdown-файлов, которые добавляют постоянные инструкции к подсказке модели в Kodify и могут автоматически подмешиваться в контекст в зависимости от файлов и их содержимого. Правила помогают зафиксировать стандарты команды (код-стиль, архитектурные требования, практики документирования), чтобы Kodify отвечал в нужном тоне и с правильными ограничениями. Rules позволяют сослаться на существующий файл с правилами в запросе к Kodify или создать новый. 

  Созданные правила можно посмотреть, нажав на кнопку "Rules" на панели Kodify, где также можно добавить новое правило.
 
  ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-rules-button.png)
  
   Визард **Rules** можно вызвать по кнопке "+ Generate Rule", которая становится доступной после завершения генерации ответа модели в чате.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-generate-rule-button.png)
   
   В визарде "Generate Rule" можно создать правило, которое
- всегда применяется ко всем файлам;
- имеет тип "auto-attached". **Auto-attached** — тип правил, которые автоматически применяются на основе шаблонов файлов; 
- запрашивается созданным агентом;
- запрашивается вручную.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/generate-rule-wizard.png)
   
   После выбора типа правила в визарде нажмите "Generate".
   В окне "Your rule" уточните значения в полях "Rule Name", "Rule Type", "Rule Content" и нажмите "Continue" для создания правила.
 
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/your-rule-window.png)
   
После отправки пользователем соответствующего запроса Kodify выдаст ответ в зависимости от выбранного действия.

Вы можете применить вариант от Kodify, используя следующие кнопки (действия) на панели с вариантом:

- **Apply** (в JetBrains) — применяет вариант от Kodify к выделенному коду.
   
    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/fix-apply-action_new.png)
   
- **Insert Code** — применяет вариант от Kodify в то место в коде, где находится курсор.
- **Copy Code/Copy** - копирует вариант от Kodify в буфер обмена.
- **Create File** — создает файл с кодом. 
- **Run** — запускает код.
- **Delete** - удаляет вариант от Kodify.
- **Helpful** и **Unhelpful** — помечают предложенный вариант как полезный или бесполезный (соответственно, лайк или дизлайк).

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/copy-code-delete-actions.png)

### Вызов функции "Объяснение кода" через меню "Quick Fix" в Visual Studio Code


В Visual Studio Code вы можете быстро получить ответ от Kodify по интересующему вас коду через меню "Quick Fix". Для этого выполните следующие действия:

1. Поставьте курсор на требуемую часть кода.
2. Откройте меню "Quick Fix" через комбинацию **"Ctrl+."** или кликните на символ "лампа" в редакторе кода.
3. Выберите пункт **"Ask Kodify"**.

    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/quick-fix-ask-kodify_new.png)

4. Окно с фрагментом кода и запросом к Kodify появится на панели. При необходимости вы можете отредактировать запрос к Kodify и затем нажать кнопку отправки запроса или **ENTER**.    

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-request.png)

   Kodify выдаст ответ по выбранной части кода.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/ask-kodify-answer_new.png)


### Вызов функций Kodify через контекстное меню в Visual Studio Code

1. Выделите код в Visual Studio Code.
2. Вызовите контекстное меню Kodify.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-context-menu.png)

3. Выберите одну из следующих функций (смотрите предыдущий скриншот):

- **Добавление выделенного кода в контекст**. Добавляет выделенный код на панель Kodify для выбора дальнейших действий.
  
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/add-selected-code.png)

- **Редактирование выделенного кода**.
- **Исправление кода**. Находит ошибки в выделенном коде и предлагает вариант исправления.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/code-correction.png)

- **Оптимизация кода**. Предлагает вариант улучшения кода.

  ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/optimization-code.png)


- **Добавление Docstring к коду**. Предлагает вариант описания назначения выделенного кода.

  ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/docstring.png)

- **Добавление комментариев к коду**. Предлагает комментарии, объясняющие строки кода. 


  ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/add-comments.png)


## Функция редактирования кода

Kodify позволяет изменять код, не покидая файл.

1. Откройте файл с кодом и выделите требуемую часть кода. Плагин предложит нажать комбинацию клавиш для функции "Edit":

   в Visual Studio Code и JetBrains — **"Ctrl+I"** для Windows или **"CMD + I"** для Mac.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/chat-edit-call.png)

   В Visual Studio Code вы также можете вызвать функцию редактирования кода, выделив код и вызвав контекстное меню Kodify. Смотрите предыдущий раздел.

2. Введите инструкции для редактирования выделенного кода в появившемся окне. Например: "Add error handling". Затем нажмите **ENTER** или кнопку отправки после запроса.  

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/add-error-handling_new.png)

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/add-error-handling_new-jetbrains.png)
   
3. Kodify проанализирует код и выделит фрагменты для изменения. Примите или отклоните предложение Kodify по изменению кода. Для принятия или отклонения конкретного выделенного фрагмента кода:

- В Visual Studio Code нажмите "Accept" или "Reject" в редакторе кода. 

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/vscode-accept-reject.png)
   

- В JetBrains нажмите "Alt+Y" или "Alt+N" в редакторе кода.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/jetbrains-accept-reject.png)

Для применения выбора ко всем фрагментам кода:

- Нажмите "Accept" или "Reject" на панели Kodify в Visual Studio Code.
- "Accept All"/"Reject All" в JetBrains в редакторе кода.

Kodify применит изменения к выделенному коду.

## Режим "Plan"

Режим "Plan" (планирование) — это ограниченная среда, которая предоставляет доступ к кодовой базе только для чтения. Он предназначен для безопасного изучения и понимания кода, а также для планирования изменений без их внесения в код.

В режиме "Plan" запрещено создавать, редактировать и удалять файлы, создавать правила и запускать команды в терминале. Можно просматривать файлы, осуществлять безопасный поиск и анализ. Доступна работа со всеми MCP инструментами, включая встроенные, но только в режиме чтения. 
Ниже приведены настройки Tools в режиме "Plan".

![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/plan-tools-settings.png)

### Установка режима "Plan"

1. Откройте панель Kodify. Чтобы открыть панель, используйте следующие комбинации клавиш:
- в Visual Studio Code — "CTRL + L" ("CMD + L" на Mac);
- в JetBrains — "CTRL+ J" ("CMD + J" на Mac).
2. Выберите режим "Plan" как показано на скриншоте ниже.
  
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/select-plan.png)

Режим "Plan" позволяет ознакомиться и изучить функциональность Kodify. Затем можно перейти в режим "Agent" для решения различных задач с помощью tools.

##  Режим "Agent"

Режим "Agent" — это специальный режим в плагине Kodify, который, благодаря использованию инструментов (tools), позволяет делегировать задачи, такие как создание файлов, написание кода, поиск контента, ввод команд и т.д. Режим "Agent" работает только с моделями, у которых есть поддержка этого режима. 

### Использование режима "Agent"

1. Откройте панель Kodify.
2. Выберите режим "Agent".

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/select-agent.png)

3. Напишите запрос, например, «Создай приложение калькулятор на языке Javascript и запусти его», и нажмите **ENTER** или кнопку отправки. Kodify предложит создать файл "calculator.html" с функциями калькулятора (сложение, вычитание, деление и умножение) и запросит подтверждение создания этого файла.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/agent-request.png)

4. Нажмите "Create file" в области с предложенным кодом.
Созданный файл откроется в редакторе кода.

    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/agent-created-file.png)

5. Прокрутите ответ модели до конца и разрешите запуск созданного Kodify приложения, нажав "Run".

    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/agent-run-code.png)

   Команда для запуска приложения появится в терминале. 

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/agent-terminal-command.png)

6. Выполните команду в терминале, чтобы запустить приложение.

    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/agent-call-application.png)
