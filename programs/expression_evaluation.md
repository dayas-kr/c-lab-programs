# 1. Evaluation of Expressions

## Aim

To evaluate an expression involving variables `x`, `y`, `z`, and `w`.

## Algorithm

1. Start
2. Prompt the user to enter values for x, y, z, and w.
3. Read the values for x, y, z, and w from the user.
4. Calculate the result using the formula `((x + y) * (x + y) * (y + z)) / w`.
5. Display the result.
6. End

## Flowchart

![Description of the image](../flowcharts/expression_evaluation.svg)

## Source Code

```c
#include <stdio.h>

int main()
{
  double x, y, z, w, result;

  printf("Enter the values of x, y, z and w: ");
  scanf("%lf %lf %lf %lf", &x, &y, &z, &w);

  result = ((x + y) * (x + y) * (x + z)) / w;

  printf("The result of the expression: %lf\n", result);

  return 0;
}
```

<!-- Go back to README -->

[Go back to all programs](../README.md)
