# 2. Temperature Conversion

## Aim

To convert temperatures from fahrenheit to celsius.

## Algorithm

1. Start
2. Prompt the user to enter the temperature in Fahrenheit.
3. Read the temperature in Fahrenheit from the user.
4. Convert the temperature from Fahrenheit to Celsius using the formula `(Fahrenheit - 32) * 5 / 9`.
5. Display the converted temperature in Celsius.
6. End

## Flowchart

![Description of the image](../flowcharts/temperature_conversion.svg)

## Source Code

```c
#include <stdio.h>

int main()
{
  float fahrenheit, celsius;

  printf("Enter the temperature in Fahrenheit: ");
  scanf("%f", &fahrenheit);

  celsius = (fahrenheit - 32) * 5 / 9;

  printf("%.2f Fahrenheit is equal to %.2f Celsius\n", fahrenheit, celsius);
  return 0;
}
```

[Go back to all programs](../README.md)
