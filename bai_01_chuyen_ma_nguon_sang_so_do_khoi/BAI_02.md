#include <stdio.h>

int main() {
    int N, i;

    printf("Nhap N: ");
    scanf("%d", &N);

    if (N < 2) {
        printf("%d khong phai so nguyen to", N);
    } else {
        i = 2;

        while (i * i <= N) {
            if (N % i == 0) {
                printf("%d khong phai so nguyen to", N);
                return 0;
            }

            i = i + 1;
        }

        printf("%d la so nguyen to", N);
    }

    return 0;
}
