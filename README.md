# Bubble-sort-Ascending-order
nnamita396-lang: #include <stdio.h>  

  

void bubbleSortAscending(int arr[], int n) {  

    int i, j, temp;  

    for (i = 0; i < n - 1; i++) {  

        for (j = 0; j < n - i - 1; j++) {  

            if (arr[j] > arr[j + 1]) {  

                // Swap  

                temp = arr[j];  

                arr[j] = arr[j + 1];  

                arr[j + 1] = temp;  

            }  

        }  

    }  

}  

  

void printArray(int arr[], int n) {  

    for (int i = 0; i < n; i++) {  

        printf("%d ", arr[i]);  

    }  

    printf("\n");  

}  

  

int main() {  

    int n, i;  

  

    printf("Enter the number of elements: ");  

    scanf("%d", &n);  

  

    int arr[n], arrCopy[n];  

  

    printf("Enter %d elements: ", n);  

    for (i = 0; i < n; i++) {  

        scanf("%d", &arr[i]);  

        arrCopy[i] = arr[i];   

    }  

  

    bubbleSortAscending(arr, n);  

    printf("Array after Bubble Sort (Ascending): ");  

    printArray(arr, n);  

  

    return 0;  

}  

