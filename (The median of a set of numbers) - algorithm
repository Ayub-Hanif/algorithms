#include <iostream>
#include <vector>

void find_the_median(int x[], int& median);

#define N 6

int main()
{
    int x[N] = { 3, 7, 1, 4, 6, 9 };
    int median;

    find_the_median(x, median);

    std::cout << median;
}
void find_the_median(int x[], int& median)
{
    int smallest_num, start_element, min_element;
    int med = (N) % 2;
    int middle = (N) / 2;

    for (int start_array = 0; start_array < (N - 1); start_array++)
    {
        min_element = start_array;
        smallest_num = x[start_array];

        for (start_element = start_array + 1; start_element < N; start_element++)
        {
            if (x[start_element] < smallest_num)
            {
                smallest_num = x[start_element];
                min_element = start_element;
            }
        }

        x[min_element] = x[start_array];
        x[start_array] = smallest_num;
    }

    if (med == 1)
    {
        median = (x[middle]);
    }
    else
    {
        median = (x[middle - 1] + x[middle + 1]) / 2;
    }
}
