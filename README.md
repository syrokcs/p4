#include <stdio.h>

int main() {
    int n;
    printf("Введіть натуральне число n: ");
    scanf("%d", &n);

    int count = 0; // Лічильник рівних дільників

    // Перевірка всіх чисел від 1 до n-1
    for (int i = 1; i < n; i++) {
        if (n % i == n / i) {
            count++;
        }
    }

    printf("Кількість рівних дільників числа %d: %d\n", n, count);

    return 0;
}
