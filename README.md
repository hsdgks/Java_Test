# Тестовое задание ЦФТ
## Сортировка слиянием, реализованная согласно [заданию](https://github.com/neko2a/cft-test-task/tree/master/docs/Java_TestTask.pdf).

### Требования к программе:
* Java 15+
* Gradle 7.1+

### Сборка:
В директории с исходниками выполнить: `gradle build`. 
После этого в папке `build/libs` появится файл `Java_TestTask-1.0.jar`.

### Параметры программы задаются при запуске через аргументы командной строки, по порядку:
1. режим сортировки (-a или -d), __необязательный__, по умолчанию сортируем по возрастанию; 
2. тип данных (-s или -i), __обязательный__;
3. имя выходного файла, __обязательное__;
4. остальные параметры - имена входных файлов, __не менее одного__.

### Примеры запуска из командной строки:
* `java -jar Java_TestTask-1.0.jar -a -i out.txt in.txt` _(для целых чисел по возрастанию)_
* `java -jar Java_TestTask-1.0.jar -s out.txt in1.txt in2.txt in3.txt` _(для строк по возрастанию)_
* `java -jar Java_TestTask-1.0.jar -d -s out.txt in1.txt in2.txt` _(для строк по убыванию)_