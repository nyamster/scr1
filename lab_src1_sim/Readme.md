# Проектирование систем на кристалле <br> Лабораторная работа №2

## Задание

Модифицировать обработку исключений в ядре `SCR1` в соответствии с вариантом задания.

Необходимо отредактировать список тестов, модифицировать обработку исключений `trap_vector`, установить параметры ядра `Reset Vector` и `Trap Vector`, а также изменить linker-скрипт для корректного запуска теста.

Вариант | Вид исключения |  Тест  | Reset Vector | Trap Vector | Обработчик
:-----: |:-------------: | :----: | :----------: | :---------: | :--------:
11  | Instruction address misaligned | `isa/rv32mi/ma_fetch.S` | 0x200 | 0x400 | Вывод строки `misalign trap`

## Результаты работы

![image](https://github.com/nyamster/scr1/blob/0fe5a27a3ac663d9b0b66a5d8c4982a41331ab85/lab_src1_sim/picture.png)

Результаты симуляции: [sim_results.txt](sim_results.txt) и [simx.vcd](simx.vcd)  
Дамп-файл теста: [ma_fetch.dump](ma_fetch.dump)
