#Практична робота №1_2: Вказівники (Частина 1)
**Виконала:** студентка групи [4СОМ] [Лучко Анастасія] (Варіант № [7])

##  Завдання.
**Завдання:** [Розробити консольну програму «Система обліку замовлень» для служби
доставки або інтернет-магазину.]
<img width="1350" height="78" alt="image" src="https://github.com/user-attachments/assets/a106451d-3a38-476a-8f35-996b04701eee" />


### 💻 Код програми:
```cpp
#include <iostream>

using namespace std;


void changePrice(double* pricePtr) {
    *pricePtr += 100;
}

int main() {
    int orderNumber = 718;
    
    
    cout << "Адреса змiнної orderNumber: \t\t" << &orderNumber << endl;
    
    int* orderNumberPtr = &orderNumber;
    
   
    cout << "Адреса через вказiвник orderNumberPtr: \t" << orderNumberPtr << endl;
    
    
    cout << "Значення змiнної orderNumber: \t\t" << orderNumber << endl;
    cout << "Значення через *orderNumberPtr: \t" << *orderNumberPtr << endl;
    
    
    *orderNumberPtr = 719; // присвоюємо нове значення
    cout << "Новий номер замовлення (через вказiвник): " << *orderNumberPtr << endl;
    cout << "------------------------------------------------" << endl;

   
    int quantity = 3;
    
    
    int* quantityPtr = &quantity;
    
    
    cout << "Початкова кiлькiсть букетiв: \t\t" << quantity << endl;
    cout << "Адреса змiнної quantity: \t\t" << &quantity << endl;
    cout << "Адреса через вказiвник quantityPtr: \t" << quantityPtr << endl;
    cout << "Значення через *quantityPtr: \t\t" << *quantityPtr << endl;
    
    *quantityPtr = 5; // клієнт, наприклад, додав ще 2 букети
    cout << "Нова кiлькiсть букетiв (через вказiвник): " << *quantityPtr << endl;
    cout << "------------------------------------------------" << endl;

  
    double price = 1350.0;
    
    
    cout << "Початкова вартiсть: \t" << price << " грн" << endl;
    
   
    changePrice(&price);
    
    
    cout << "Нова вартiсть (+100 грн): \t" << price << " грн" << endl;

    return 0;
}
```
### 👁️ Візуалізація пам'яті:
<img width="1208" height="675" alt="image" src="https://github.com/user-attachments/assets/8863914e-0b1e-45fc-9779-24c35b226c32" />
<img width="1203" height="659" alt="image" src="https://github.com/user-attachments/assets/6f6d7ac2-778b-4c92-a407-b86b5fd39ddc" />
<img width="1147" height="668" alt="image" src="https://github.com/user-attachments/assets/b111438a-06dc-4abc-acc0-5c2dc3ba1d5f" />
<img width="1180" height="664" alt="image" src="https://github.com/user-attachments/assets/a0daeb36-7fa4-4fed-bc7c-5a8c02b18321" />
<img width="1211" height="722" alt="image" src="https://github.com/user-attachments/assets/b5adcf29-2917-43a1-bc21-f39117c1c3f8" />





