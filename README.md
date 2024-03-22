#include <iostream>
using namespace std;

void  FillArray(int const arr, int const size)
{
    for (int i = 0; i < size; i++)
    {

        arr[i] = rand() % 10;

    }


}
void ShowArray(const intarr, int const size)
{
    for (int i = 0; i < size; i++)
    {

        cout << arr[i] << "\t";


    }
    cout << endl;

}

void push_back(int &arr, int &size, const int value)
{

    intnewArray = new int[size + 1];
    for (int i = 0; i < size; i++)
    {


        newArray[i] = arr[i];
    }
    newArray[size] = value;

    size++;

    delete[]arr;

    arr = newArray;


}
void pop_back(int &arr, int &size)
{
    size--;
    intnewArray = new int[size];
    for (int i = 0; i < size; i++)
    {

        newArray[i] = arr[i];


    }



}

void main()
{


    int size = 5;
    int* arr = new int[size];
    FillArray(arr, size);

    ShowArray(arr, size);

    push_back(arr, size, 111);

    ShowArray(arr, size);


    pop_back(arr, size);

    ShowArray(arr, size);

    delete[]arr;


}

//nika that's for u, you can start building Rest api for F.T
