# 3. Day Count to Months and Days

## Aim

To convert days to months and days.

## Algorithm

1. Start
2. Prompt the user to enter the number of days.
3. Read the number of days from the user.
4. Calculate the number of months by dividing the number of days by 30.
5. Calculate the number of remaining days by taking the modulus of the number of days with 30.
6. Display the number of months and remaining days.
7. End

## Flowchart

![Description of the image](../flowcharts/day_count_to_months_days.svg)

## Source Code

```c
#include <stdio.h>

int main()
{
  int days, rem_months, rem_days;

  printf("Enter the number of days: ");
  scanf("%d", &days);

  rem_months = days / 30;
  rem_days = days % 30;

  printf("%d days is equal to %d months and %d days\n", days, rem_months, rem_days);
  return 0;
}
```

[Go back to all programs](../README.md)
