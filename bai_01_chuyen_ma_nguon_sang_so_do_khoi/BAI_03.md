#include <stdio.h>

int main() {
    int n;
    printf("Nhap n: ");
    scanf("%d", &n);
    
    int A[n];
    for(int k = 0; k < n; k++) {
        printf("Nhap A[%d]: ", k);
        scanf("%d", &A[k]);
    }
    
    int Lon_nhat = A[0];
    int i = 1;
    
    while(i < n) {
        if(A[i] > Lon_nhat) {
            Lon_nhat = A[i];
        }
        i = i + 1;
    }
    
    printf("So lon nhat la: %d\n", Lon_nhat);
    return 0;
}
