#include <iostream>
using namespace std;

int findsmallest(int arr[], int size) { 
    int smallest = arr[0]; 
    for (int i = 1; i < size; i++) { 
        if (arr[i] < smallest) {  
            smallest = arr[i]; 
        } 
    } 
    return smallest; 
} 

int main() { 
    int arr[] = {10, 2, 30, 40, 5}; 
    int size = sizeof(arr) / sizeof(arr[0]); 
    int smallest = findsmallest(arr, size); 
    cout << "The smallest number in the array is: " << smallest << endl; 
    return 0; 
}

