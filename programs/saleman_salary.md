# 4. Saleman Salary

## Aim

Calculate the total salary of a salesman based on the basic salary, bonus per item sold, number of items sold, total sales amount, and commission rate per item sold.

## Algorithm

1. **Start**
2. Prompt the user to enter the **basic salary** and store it in `basic_salary`.
3. Prompt the user to enter the **bonus per item sold** and store it in `bonus`.
4. Prompt the user to enter the **number of items sold** and store it in `items_sold`.
5. Prompt the user to enter the **total sales amount** and store it in `total_sales`.
6. Prompt the user to enter the **commission rate per item sold** and store it in `commission_rate`.
7. **Calculate the total bonus**:
   - `bonus_amount = bonus * items_sold`
8. **Calculate the total commission**:
   - `commission_amount = total_sales * commission_rate`
9. **Calculate the total salary**:
   - `total_salary = basic_salary + bonus_amount + commission_amount`
10. Display the **bonus amount**.
11. Display the **commission amount**.
12. Display the **total salary**.
13. **End**

## Flowchart

![Description of the image](../flowcharts/saleman_salary.svg)

## Source Code

```c
#include <stdio.h>

int main()
{
  float basic_salary, bonus, commission, total_sales;
  float bonus_ammount, commission_amount, total_salary;
  int item_sold;

  printf("Enter the basic salary: ");
  scanf("%f", &basic_salary);
  printf("Enter bonus per item sold: ");
  scanf("%f", &bonus);
  printf("Enter numbers of items sold: ");
  scanf("%d", &item_sold);
  printf("Enter total sales amount: ");
  scanf("%f", &total_sales);
  printf("Enter commission per item sold: ");
  scanf("%f", &commission);

  bonus_ammount = bonus * item_sold;
  commission_amount = total_sales * (commission / 100);
  total_salary = basic_salary + bonus_ammount + commission_amount;

  printf("\nBonus Ammount: %.2f\n", bonus_ammount);
  printf("Commission Ammount: %.2f\n", commission_amount);
  printf("Total Salary: %.2f\n", total_salary);
  return 0;
}
```

[Go back to all programs](../README.md)
