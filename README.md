# Algoficient-Materials

#include <stdio.h>

int main() {

    // 2D ARRAY PRACTICE < intergers >
    // int N;
    // scanf("%d", &N); getchar();
    
    // int array[N][N];
    // for(int i = 0; i < N; i++){
    //     for(int j = 0; j < N; j++){
    //         scanf("%d", &array[i][j]); getchar();
    //     }
    // }
    
    // for(int i = 0; i < N; i++){
    //     for(int j = 0; j < N; j++){
    //         printf("%d ", array[i][j]);
    //     }
    //     printf("\n");
    // }

    // 2D ARRAY PRACTICE < characters >
    int N;
    scanf("%d", &N); getchar();
    int x, y;
    
    char matrix[N][N+5];
    for(int i; i < N; i++){
        for(int j = 0; j < N; j++){
            scanf("%c", &matrix[i][j]);
        }
        getchar();
    }
    
    for(int i = 0; i < N; i++){
        for(int j = 0; j < N; j++){
            if(matrix[i][j] == '*'){
                y = i + 1;
                x = j + 1;
            }
        }
    }
    
    printf("%d, %d", x, y);
    
    
    return 0;
}
