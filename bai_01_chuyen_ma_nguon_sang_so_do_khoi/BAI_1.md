#include <stdio.h>
#include <math.h>

int main() {
    float a, b, c;
    float delta, x, x1, x2;
    printf("Nhap a, b, c: ");
    scanf("%f%f%f", &a, &b, &c);

    if (a == 0) {
        if (b == 0) {
            if (c == 0) {
                printf("Vo so nghiem");
            } else  {
                printf("Vo nghiem");
            }
        } else {
            x = -c / b;
            printf("Phuong trinh co nghiem x = %.2f", x);
        }
    } else {
        delta = b * b -4 * a *c;

        if (delta < 0) {
          printf("Vo nghiem");
        } else if (delta == 0) {
            x1 = -b / (2 * a);
            x2 = x1;

            printf("Nghiem kep x1 = x2 = %.2f", x1);
        } else {
            x1 = (-b + sqrt(delta)) / (2 *a);
            x2 = (-b - sqrt(delta)) / (2 *a);

            printf("x1 = %.2f\n", x1);
            printf("x2 = %.2f", x2);
        }
      }

      return 0;
            
