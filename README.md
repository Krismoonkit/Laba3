#include <iostream>
#include <vector>

using namespace std;

int main() {
    setlocale(LC_ALL, "Russian");
    
    vector<int> numbers;
    
    // Проверяем, заполнен ли вектор 10 элементами
    if (numbers.size() == 10) {
        cout << "Вектор заполнен 10 элементами!" << endl;
        cout << "Элементы вектора: ";
        for (int num : numbers) {
            cout << num << " ";
        }
        cout << endl;
    } 
    // Проверяем, пустой ли вектор
    else if (numbers.empty()) {
        cout << "Вектор пустой! Добавляем 3 элемента..." << endl;
        numbers.push_back(1);
        numbers.push_back(2);
        numbers.push_back(3);
        
        cout << "После добавления 3 элементов:" << endl;
        cout << "Размер вектора: " << numbers.size() << endl;
        cout << "Элементы: ";
        for (int num : numbers) {
            cout << num << " ";
        }
        cout << endl;
    }
    else {
        cout << "Вектор содержит " << numbers.size() << " элементов." << endl;
        cout << "Элементы: ";
        for (int num : numbers) {
            cout << num << " ";
        }
        cout << endl;
    }
    
    return 0;
}
