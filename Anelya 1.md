num1 = float(input("Введите первое число: "))
num2 = float(input("Введите второе число: "))

operation = input("Выберите операцию (+, -): ")

if operation == "+":
    result = num1 + num2
elif operation == "-":
    result = num1 - num2

    if num2 != 0:
        result = num1 / num2
    else:
        print("Ошибка: деление на ноль!")
        result = None
else:
    print("Некорректный ввод. Пожалуйста, введите +, -, * или /.")
    result = None

if result is not None:
    print("Результат:", result)
