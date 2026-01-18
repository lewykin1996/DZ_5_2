# DZ_5_2 (Максимум и минимум)

// Вывод массива на экран.cpp : Этот файл содержит функцию "main". Здесь начинается и заканчивается выполнение программы.
//

#include <iostream>
#include <string>
using namespace std;

int main()
{
  setlocale(LC_ALL, "Russian");

  int arr[10] = { 5, 6, 7, 8, 60, 10, 11, 12, 13, 14 };

  int min = arr[0];
  int max = arr[0];

  cout << '\n' << endl;

  cout << "Массив:" << '\t';
  for (int i = 0; i < 10; i++)
  {
    cout << arr[i] << '\t';

    if (arr[i] < min)
    {
      min = arr[i];
    }

    if (arr[i] > max)
    {
      max = arr[i];
    }

  }
  cout << '\n' << endl;

  cout << "Минимальный элемент: " << min << '\n' << endl;
  cout << "Максимальный элемент: " << max << endl;

  return 0;
}
