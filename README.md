# ya CheckStyle
code style validation for yandex java backend course

Как проверить стиль кода локально , дабы избежать лишних комитов с исправлениями.
1. Качаем проверялку [тут](https://github.com/checkstyle/checkstyle/releases/)
   ![проверялка](/download.PNG)

2. качем конфиги [тут](https://github.com/yandex-praktikum/java-filmorate/tree/controllers-films-users)
   нас интересуют файлы **checkstyle.xml** и **suppressions.xml**
   ![конфиги](/configs.PNG)

3. складываем все в 1 любую папку локально, лучше выделить отдельную папку для проверок и не пихать себе в реп.
   ![папко](/folder.PNG)

4. запускаем через командную строку проверку файла
   ```
   java -jar checkstyle-10.14.2-all.jar -c checkstyle.xml AwesomeCode.java
   ```
   ![проверка](/command.PNG)

5. исправляем очепятки!


мопед не мой. авторы и сам приклад тут https://checkstyle.org/
в инструкции самый простой сценарий. По факту проверка доступна и в виде плагина к IDE (помимо интеграции с github actions)
