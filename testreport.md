# Отчёт о тестировании приложения Precision

## Краткое описание

Необходимо создать программу, которая рассчитывает дополнительный бонус для новых клиентов.

Входные данные:
```java
public class Main {
  public static void main(String[] args) {
    double regularBonus = 0.3;
    double specialBonus = 0.6;
    double totalBonus = regularBonus + specialBonus;
    System.out.println(totalBonus);
  }
}
```

## Описание тестов

Было проведено позитивное функциональное тестирование.

1. Смоделировать требуемую функцию через следующий код:
```java
public class Main {
  public static void main(String[] args) {
    double regularBonus = 0.3;
    double specialBonus = 0.6;
    double totalBonus = regularBonus + specialBonus;
    System.out.println(totalBonus);
  }
}
```
2. Запустить код и проверить вывод.

## Результаты
В результате моделирования функции вывода результата расчета дополнительного бонуса обнаружен следующий баг:



## Общие рекомендации

Необходимо обратить внимание на количество знаков после запятой в переменной totalBonus.
Тип double при вычислении возвращает число с большим количеством знаков после запятой, что не совсем подходит для использования в финансовой сфере, где логичным будет округлять значение до двух знаков после запятой.
