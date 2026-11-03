#include <stdio.h>

int main() {
    int N, i;

    printf("Nhap N: ");
    sacnf("%d", &N);

    if (N < 2) {
        printf("%d khong phai so nguyen to", N);
