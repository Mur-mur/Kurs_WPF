# Предисловие
Программа предназначена для шифрования/дешифрования текста с помощью Шифра Виженера

# Функциональные возможности
Для данного решения была использована WPF технология.

Программа обладает следующими возможностями:  
- Шифрование/Дешифрование текста, введенного с клавиатуры, используя ключ.  
- Шифрование/Дешифрование текста, загруженного из текстового файла .txt или .docx, используя ключ.  
- Экспорт шифрованного/дешифрованного текста в файл в формате .txt / .docx  
- При открытии .txt файла программа автоматически выбирает подходящую кодировку (ANSI | UTF8).

В качестве дополнительных опций, доступных пользователю:  
- Сохранение регистра букв после выполнения операции  
- Перевод расшифрованного текста в формат регистра "Как в предложении."  

# Описание интерфейса
Главная страница приложения.  
В ней располагаются блоки:  
- Ввода ключа.  
- Двух полей для ввода текста.  
- Переключения режима работы.  
- Дополнительные функции.  

![](https://github.com/Mur-mur/Kurs_WPF/blob/master/Description%20Pictures/MainWindow.png)

По умолчанию выбрано шифрование текста, для переключения на расшифровку необходимо нажать соответствующую кнопку. Шифруются только буквы русского алфавита, остальные сиволы остаются без изменений.  
![](https://github.com/Mur-mur/Kurs_WPF/blob/master/Description%20Pictures/Change.png)  

Для корректного осуществления базовых операций пользователю необходимо ввести ключ в соответствующее поле.  
Ключ может состоять из любых символов, однако при замене в шифровании учитываются только русские буквы, дешифруя/шифруя очередной символ при нахождении в текущей позиции ключа отличного от русского алфавита символа, программа оставит текущую букву неизменной.  
![](https://github.com/Mur-mur/Kurs_WPF/blob/master/Description%20Pictures/Key.png) 

В текстовые поля пользователь может вводить текст с клавиатуры, а так же вставлять его с помощью кнопки "Открыть".
Текст будет вставлен в текущее выбранное поле, а в случае невозможности, соответственно выбранному переключателю Зашифровать/Расшифровать.  
![](https://github.com/Mur-mur/Kurs_WPF/blob/master/Description%20Pictures/Open.png)  

Для экспорта текста из поля в файл необходимо нажать кнопку "Экспорт" на панели инструментов.  
![](https://github.com/Mur-mur/Kurs_WPF/blob/master/Description%20Pictures/Export.png)  

Пользователю доступны две опции:  
- Оставить буквы заглавными. При её активации в после выполнения операции регистр будет оставаться таким как в оригинале ( по умолчанию регистр всегда нижний).  
- В расшифрованном тексте регистр букв будет по правилам заглавных букв в тексте.  

![](https://github.com/Mur-mur/Kurs_WPF/blob/master/Description%20Pictures/Register.png)  

Для запуска шифрования/дешифрования можно нажать кнопку "Выполнить", что осуществит выбранную операцию, а так же воспользоваться кнопками Шифровать/Дешифровать на панели инструментов.  
![](https://github.com/Mur-mur/Kurs_WPF/blob/master/Description%20Pictures/Execute.png)  
![](https://github.com/Mur-mur/Kurs_WPF/blob/master/Description%20Pictures/Encrypt-Decrypt.png)  

# Unit-тесты
Основной функционал покрыт unit-тестами с использованием MsTest:  
- Ключ шифрования  
- Шифрование/Дешифрование  
- Импорт/Экспорт  
- Дополнительные пользовательские функции  

