# Отчёт о тестировании модуля сложения

### В модуле реализована функциональность суммирования текущего баланса и входящего перевода.

15.06.2021 - 15.06.2021 было проведено функциональное тестирование модуля.

На тестирование затрачено: 1 час.

### В результате тестирования выявлены следующие дефекты:

* [Ошибка при расчете итоговой суммы при сложении значений текущего баланса и суммы поступления. #1](https://github.com/leonidbeltsov/JavaTask2.1/issues/1)

### Описание процесса тестирования

#### Входные данные:
* текущий баланс счёта клиента - переменная типа int, значение - 2_000_000_000 (два миллиарда) рублей  

* сумма перевода - переменная типа int, значение - 500_000_000 (пятьсот миллионов) рублей  

* переменная для хранения итогового значения - тип int

#### Ожидаемый результат:  

* Итоговая сумма равная 2_500_000_000 (два миллиарда пятьсот миллионов) рублей

#### Фактический результат:
* Ошибка приложения при выводе итоговой суммы c выводом следующего сообщения:
> "C:\Program Files\AdoptOpenJDK\jdk-11.0.11.9-hotspot\bin\java.exe" -javaagent:C:\Users\HP\AppData\Local\JetBrains\Toolbox\apps\IDEA-C\ch-0\211.7442.40\lib\idea_rt.jar=55972:C:\Users\HP\AppData\Local\JetBrains\Toolbox\apps\IDEA-C\ch-0\211.7442.40\bin -Dfile.encoding=UTF-8 -classpath C:\Users\HP\IdeaProjects\JavaTask2.1\out\production\JavaTask2.1 Main  
-1794967296

#### Тестирование производилось в следующем окружении:
* Windows 10 Домашняя (x64)  
  Версия  21H1  
  Сборка ОС	19043.1052  

* openjdk version "11.0.11" 2021-04-20  
  OpenJDK Runtime Environment AdoptOpenJDK-11.0.11+9 (build 11.0.11+9)  
  OpenJDK 64-Bit Server VM AdoptOpenJDK-11.0.11+9 (build 11.0.11+9, mixed mode)  

* IntelliJ IDEA 2021.1.2 (Community Edition)  
  Build #IC-211.7442.40, built on June 1, 2021  
  Runtime version: 11.0.11+9-b1341.57 amd64