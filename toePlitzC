#include <stdio.h>
#include <stdbool.h>

bool is_toeplitz(int matrix[][4], int rows, int cols) {
    for (int i = 1; i < rows; i++) {
        for (int j = 1; j < cols; j++) {
            if (matrix[i][j] != matrix[i-1][j-1]) {
                return false;
            }
        }
    }
    return true;
}

int main() {
    int matrix[4][4] = {
        {1, 2, 3, 4},
        {5, 1, 2, 3},
        {6, 5, 1, 2},
        {7, 6, 5, 1}
    };

    int rows = 4;
    int cols = 4;

    if (is_toeplitz(matrix, rows, cols)) {
        printf("The matrix is a Toeplitz matrix.\n");
    } else {
        printf("The matrix is not a Toeplitz matrix.\n");
    }

    return 0;
}
