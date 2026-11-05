#include <stdio.h>

int main() {
    int a, b, x, y, z;
    int UCLN, BCNN;

    printf("Nhap a, b: ");
    scanf("%d%d", &a, &b);

    x = a;
    y = b;

    while (y != 0) {
        z = x % y;
        x = y;
        y = z;
    }

    UCLN = x;
    BCNN = a * b / UCLN;

    printf("UCLN = %d\n", UCLN);
    printf("BCNN = %d\n", BCNN);

    return 0;
}
