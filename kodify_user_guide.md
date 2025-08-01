# Перечень терминов

**Таблица 1**. Термины, используемые в руководстве **Kodify**.

| Термин | Описание | 
|-------|-----|
|Генерация кода| Автоматическое создание программного кода специальным приложением (генератором кода) по заданным условиям. |
|Искусственный интеллект| Область компьютерных наук, занимающаяся созданием вычислительных систем, способных выполнять задачи, требующие человеческого интеллекта, такие как восприятие, рассуждение, обучение и решение проблем. |
|Токен| Минимальная единица текста, например, слово или символ. Применяется в обработке естественного языка для анализа и генерации текста. |
|Unit тест | Проверка на корректность работы отдельных модулей исходного кода программы (функций, методов, классов). |



# Перечень сокращений

**Таблица 2**. Сокращения в руководстве **Kodify**.

| Сокращение | Описание | 
|-------|-----|
|ПО| Программное обеспечение |
|AI (Artificial Intelligence)| Интеллект, демонстрируемый машинами, в частности компьютерными системами. |
|IDE (Integrated Development Environment)| Программа, в которой разработчики пишут, проверяют, тестируют и запускают код, а также ведут большие проекты. |
|JSON (JavaScript Object Notation)| Лёгкий формат обмена данными. Формат легко читается человеком и парсируется компьютером. |
|LLM (Large Language Model)| Языковая модель, состоящая из нейронной сети со множеством параметров. |
|UI (User Interface)| Пользовательский интерфейс. |


# Введение

Настоящий документ представляет собой руководство пользователя (далее руководство) системы Kodify.

Руководство описывает:
- общее определение системы;
- функции системы;
- настройку и установку плагина в среде Visual Studio Code;
- настройку и установку плагина в среде JetBrains;
- работу с плагином.

## Краткое описание возможностей

Kodify от MWS AI представляет собой AI-ассистента разработчика. Этот инструмент использует искусственный интеллект для автоматизации рутинных процессов и помощи разработчикам в выполнении различных задач при написании программного кода. 

Функции Kodify:

- Автопродление кода с помощью LLM, которая на основе уже написанного пользователем кода генерирует завершение строки.
- Документирование кода
- Поиск ошибок в коде и исправление найденных ошибок.
- Формирование Unit-тестов для кода пользователя.
- Объяснение кода.

## Уровень подготовки пользователей

Пользователи Системы должны:

- обладать базовыми навыками работы в IDE в средах Visual Studio Code или JetBrains; 
- знать один из популярных языков программирования (например, Python, C#, Java, Go, JavaScript).

## Перечень эксплуатационной документации, с которой необходимо ознакомиться пользователю

Для работы в Системе, пользователь должен ознакомиться с настоящим руководством.

# Назначение и условия применения

Система предназначена для облегчения процесса разработки, предоставляя инструменты для генерации кода, улучшения его качества и автоматизации рутинных задач. Kodify поддерживает различные языки программирования (например, Python, C#, Java, Go, JavaScript) и интеграции с популярными инструментами разработки.

Kodify представляет собой LLM и плагин, встраиваемый в IDE. Взаимодействие пользователя с LLM Kodify осуществляется через пользовательский интерфейс (UI) в виде плагина. Плагин содержит набор функций для упрощения и ускорения процесса написания кода за счёт обращения к LLM. Плагин доступен для Visual Studio Code и JetBrains IDE's.

# Подготовка к работе

## Установка плагина в среде Visual Studio Code

> Поддерживаются среды разработки Visual Studio Code и IntelliJ IDEA.

1. Скачайте последнюю версию плагина Kodify для Visual Studio Code. Ссылку для скачивания предоставит сотрудник MWS AI.
2. Перейдите в раздел **"Extensions"** на левой панели инструментов.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/extensions.png)
   
3. В диалоговом меню выберите пункт **"Install from VSIX…"** и укажите скачанный файл плагина.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/install-from-vsix.png)
   

## Установка плагина в среде JetBrains

1. Скачайте последнюю версию плагина Kodify для JetBrains. Ссылку для скачивания предоставит сотрудник MWS AI.
2. Запустите IDE и перейдите в настройки IDE.
3. Напишите в поиске plugins или выберите пункт "Plugins" для перехода в настройку плагинов.
   
    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/pycharm_plugins.png)

  
4. Нажмите на шестеренку в правом верхнем углу и выберите **"Install Plugin from Disk…"**.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/install-plugin-from-disk.png)
   
5. Выберите скачанный файл с плагином.
6. Подтвердите перезагрузку IDE после установки. Нажмите **"Restart IDE"**.

## Настройка плагина в средах Visual Studio Code и JetBrains

1. Откройте в IDE любой файл.
2. Откройте боковую панель Kodify, используя следующую комбинацию клавиш:
  - в Visual Studio Code - **"CTRL + L"** (**"CMD + L"** на Mac);
  - в JetBrains - **"CTRL+ J"** (**"CMD + J"** на Mac).

    На следующем скриншоте показана боковая панель "Kodify" в Visual Studio Code.
    
     ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/vscode-kodify-panel.png)
    
    Боковая панель "Kodify" в JetBrains выглядит следующим образом:    
    
     ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/jetbrains-kodify-panel.png)
    
3. Откройте конфигурационный файл *config.json* одним из следующих способов:

   **Способ 1**

   На боковой панели Kodify нажмите на кнопку **"Open Settings"** в Visual Studio Code
   
    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/vscode-open-settings-button.png)
   
   или **"Kodify Сonfig"** в JetBrains.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/jetbrains-kodify-config-button.png)

   
   В разделе Configuration для Chat настроек нажмите кнопку **"Open Config File"**.
   
    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/open-config-file-button.png)
   
   
   **Способ 2**

   На боковой панели, раскройте меню Kodify и нажмите на кнопку **"Open Settings"** (шестеренка).
   
    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-open-settings-button.png)
       
   > После установки плагина Kodify, в IDE JetBrains могут быть неактивны кнопки открытия конфигурационного файла *config.json*. Для изменения состояния этих кнопок, переключите фокус с IDE, нажав **"Alt+Tab"**. Затем, верните фокус обратно в IDE. Нажмите снова **"Alt+Tab"**.

4. Заполните конфигурационный файл *config.json*.

   Если вы планируете обращаться к Kodify в контуре MWS AI, то в конфигурационном файле для плагина вам необходимо указать **baseUrl** (адрес сервера, к которому вы будете обращаться) и **токен**, который будет использоваться плагином при отправке API-запросов к серверу. Для получения **baseUrl** и **токена** обратитесь к сотруднику MWS AI.

   **baseUrl** и **токен** требуется указать трижды:
  - в разделе **"models"** - поля **"apiBase"** и **"apiKey"**;
  - в разделе **"tabAutocompleteModel"** - поля **"apiBase"** и **"apiKey"**;
  - в разделе **"embeddingsProvider"** - поля **"apiBase"** и **"apiKey"**.

    Если в контуре вашей компании развёрнут отдельный экземпляр Kodify, то помимо **baseUrl** и **токена** вам потребуется заполнить в конфигурационном файле поле **"model"** (id модели) в следующих разделах:
  - в разделе **"models"**;
  - в разделе **"tabAutocompleteModel"**;
  - в разделе **"embeddingsProvider"**.

5. Сохраните настройки файла *config.json* в IDE. Для этого, нажмите комбинацию клавиш **"Ctrl+S"** или выберите пункт меню IDE: **File** -> **Save**.

# Работа с плагином 

> Плагин настроен и готов к работе. Сервис подключится автоматически (при необходимости перезагрузите IDE). 

## Автоматическое дополнение кода

Функция автодополнение кода предлагает вероятный вариант продолжения кода по мере его ввода пользователем в редакторе кода IDE.

1. Откройте любой файл с Python-кодом или иным языком программирования.
2. Поставьте курсор, например, после **"for i in range(len(x)):"** (смотрите скриншот ниже) и нажмите **ENTER**. Kodify предложит вариант дополнения кода.
   
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/autocompletion-code-suggestion.png)
   
3. Нажмите **TAB**, чтобы принять предложенное дополнение кода.
   
    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/autocompletion-code-applied.png)     

4. Если требуется продолжить автодополнение, нажмите **ENTER** еще раз и повторите шаг 3.

> Если возникли проблемы при установке или настройке, пожалуйста, свяжитесь с нами удобным способом, и мы обязательно поможем.

## Функциональность помощника разработчика

Kodify помогает разработчикам получить справочную информацию о выделенном коде, не покидая IDE.

1. Откройте файл с кодом и выделите требуемую часть кода. Плагин предложит нажать комбинацию клавиш:
- в Visual Studio Code - **"Ctrl+L"** для Windows или **"CMD + L"** для Mac;
- в JetBrains - **"Ctrl+J"** для Windows или **"CMD + J"** для Mac.

  ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/vscode-select-code.png)     
  
2. В открывшемся окне введите знак **"/"**. Появятся доступные варианты:
- **/docs** - добавляет docstring к выделенной части кода;
- **/test** - генерирует Unit-test к выделенной части кода;
- **/fix** - ищет и исправляет ошибки в выделенной части кода;
- **/explain (rus)** - объясняет что делает код на русском языке.

  ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/plugin-functions.png)     
  
  Также, вместо использования одного из преднастроенных вариантов, вы можете самостоятельно описать те действия, которые Kodify должен будет произвести с выделенной частью кода.

3. Выберите нужный вам вариант или опишите собственный и нажмите на кнопку отправки или **ENTER**.
  
   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-send-request.png)   
      
   После отправки пользователем соответствующего запроса, Kodify выдаст ответ. 

   На следующем скриншоте показан фрагмент ответа на вариант **"/explain  (rus)"**:
   
    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-explain-function.png)
    
Вы можете применить вариант от Kodify, используя следующие кнопки (действия) на панели с вариантом:
- **Apply** - применяет вариант от Kodify к выделенному коду.
   
    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/fix-apply-action.png)
   
- **Insert at cursor** - применяет вариант от Kodify к месту в коде, где стоит курсор. 
- **Copy** - копирует вариант от Kodify в буфер.
- **Delete** - удаляет вариант от Kodify.
  
    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/fix-delete-action.png)
   
- **Helpful** и **Unhelpful** - помечают предложенный вариант как лайк или дизлайк.

### Вызов функции "Объяснение кода" через меню "Quick Fix"

В Visual Studio Code вы можете, через меню "Quick Fix", быстро получить ответ от Kodify по интересующему вас коду. Для этого выполните следующие действия:
1. Поставьте курсор на требуемую часть кода.
2. Откройте меню "Quick Fix" через комбинацию **"Ctrl+."** или кликните на символ "лампа" в редакторе кода.
3. Выберите пункт **"Ask Kodify"**.

    ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/quick-fix-ask-kodify.png)

   Kodify выдаст ответ по выбранной части кода.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/ask-kodify-answer.png)


### Вызов функций Kodify через контекстное меню для Visual Studio Code

1. Выделите интересующий вас код в Visual Studio Code.
2. Вызовите контекстное меню Kodify.
3. Выберите одну из следующих функций (смотрите скриншот внизу):
- Добавление выделенного кода в контекст;
- Исправление кода;
- Оптимизация кода;
- Добавление Docstring для кода;
- Добавление комментариев для кода.

![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/vscode-kodify-context-menu.png)


## Функция редактирования кода

Kodify позволяет вам изменить код, не покидая файл.

1. Откройте файл с кодом и выделите требуемую часть кода. Плагин 
предложит нажать комбинацию клавиш:

   в Visual Studio Code и JetBrains - **"Ctrl+I"** для Windows или **"CMD + I"** для Mac.

2. Опишите какие изменения Kodify следует внести в код.
Например, "Add error handling". Затем, нажмите **ENTER** или, после запроса, нажмите кнопку отправки.  

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/add-error-handling.png)
   
3. Kodify проанализирует код и выделит фрагменты для его изменения.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/kodify-code-analysis.png)
   
4. Примите или отклоните предложение от Kodify по изменению кода. 

   Для принятия или отклонения конкретного выделенного фрагмента кода, нажмите **"Accept"** или **"Reject"** в редакторе кода.

   Для применения выбора ко всем фрагментам кода, нажмите **"Accept"** или **"Reject"** на панели Edit Mode в Visual Studio Code или **"Accept All"**/**"Reject All"** в JetBrains.

   ![](https://raw.githubusercontent.com/mts-ai/kodify/main/images_user_guide/accept-reject-suggestion.png)
      
Kodify применит изменение к выделенному коду.