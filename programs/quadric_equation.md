# 5. Quadratic Equation Solver

## Aim

To solve a quadratic equation by finding its roots, determining whether they are real and different, real and the same, or complex, based on the coefficients.

## Algorithm:

1. **Start**
2. Prompt the user to enter the coefficients a, b, and c.
3. Calculate the discriminant using the formula: `discriminant = b^2 - 4 * a * c`.
4. Check the value of the discriminant:
   - If the `discriminant > 0`, the roots are real and different:
     - Calculate `root1 = (-b + square root of discriminant) / (2 * a)`
     - Calculate `root2 = (-b - square root of discriminant) / (2 * a)`
     - Print root1 and root2 as real and different.
   - If the `discriminant == 0`, the roots are real and the same:
     - Calculate `root1 = root2 = -b / (2 * a)`
     - Print root1 and root2 as real and the same.
   - If the discriminant is less than 0, the roots are complex and different:
     - Calculate `real part = -b / (2 * a)`
     - Calculate `imaginary part = square root of (-discriminant) / (2 * a)`
     - Print root1 and root2 with the real part and imaginary part.
5. **End**

## Flowchart

![Description of the image](../flowcharts/quadric_equation.svg)

## Source Code

```c
#include <stdio.h>
#include <math.h>

int main()
{
  float a, b, c, discriminant, root1, root2, real_part, img_part;

  printf("Enter the coefficients a, b, and c: ");
  scanf("%f%f%f", &a, &b, &c);

  discriminant = b * b - 4 * a * c;

  if (discriminant > 0)
  {
    root1 = (-b + sqrt(discriminant)) / (2 * a);
    root2 = (-b - sqrt(discriminant)) / (2 * a);
    printf("\nINFO: The roots are real and different.\n");
    printf("Root 1: %.2f\n", root1);
    printf("Root 2: %.2f\n", root2);
  }
  else if (discriminant == 0)
  {
    root1 = root2 = -b / (2 * a);
    printf("\nINFO: The roots are real and same.\n");
    printf("Root 1: %.2f\n", root1);
    printf("Root 2: %.2f\n", root2);
  }
  else
  {
    real_part = -b / (2 * a);
    img_part = sqrt(-discriminant) / (2 * a);
    printf("\nINFO: The roots are complex and different.\n");
    printf("Root 1: %.2f + %.2f i\n", real_part, img_part);
    printf("Root 2: %.2f - %.2f i\n", real_part, img_part);
  }

  return 0;
}
```

[Go back to all programs](../README.md)
