#include <iostream>
using namespace std;

void insertElement(int *arr, int &size, int max) {
    int index, num;
    cout << "Enter number to insert: ";
    cin >> num;
    cout << "Enter index (0-" << max - 1 << "): ";
    cin >> index;
    if (index < 0 || index > size || size >= max) {
        cout << "Error! Invalid index.\n";
        return;
    }
    for (int i = size; i > index; i--) {
        arr[i] = arr[i - 1];
    }
    arr[index] = num;
    size++;
}

void deleteElement(int *arr, int &size) {
    int index;
    cout << "Enter index to delete (0-" << size - 1 << "): ";
    cin >> index;
    if (index < 0 || index >= size) {
        cout << "Error! Invalid index.\n";
        return;
    }
    for (int i = index; i < size - 1; i++) {
        arr[i] = arr[i + 1];
    }

    size--;
}

int main() {
    const int max = 10;
    int arr[max] = {5, 4, 3, 2, 1};
    int size = 5;
    insertElement(arr, size, max);
    deleteElement(arr, size);
    cout << "Array: ";
    for (int i = 0; i < size; i++) {
        cout << arr[i] << " ";
    }
    cout << endl;

    return 0;
}
