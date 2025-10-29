
#include <stdio.h>

int main() {
    int a, b, temp;

    // Saisie des deux nombres
    printf("Entrez deux nombres entiers : ");
    scanf("%d %d", &a, &b);

    // Algorithme d'Euclide
    while (b != 0) {
        temp = b;
        b = a % b;
        a = temp;
    }

    printf("Le PGCD est : %d\n", a);

    return 0;
}
