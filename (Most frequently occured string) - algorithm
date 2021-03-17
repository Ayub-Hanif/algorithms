#include <iostream>
#include <vector>

std::string More_repeated(std::vector<std::string> Names, int n)
{
    std::string mode;
    std::vector<std::string> repeated_ones;
    std::vector<int> num_repeted;
    num_repeted.assign(n, 0);

    for (int i = 0; i < n; i++)
    {
        repeated_ones.push_back(Names[i]);
    }
    for (int z = 0; z < n; z++)
    {
        for (int i = 1; i < n; i++)
        {
            if (Names[i] == repeated_ones[z])
            {
                num_repeted.at(i) += 1;
            }
            if (num_repeted[i] > num_repeted[z])
            {
                mode = repeated_ones[i];
            }
        }
    }
    //The mode is the value that occurs most frequently.
    return mode;
}

int main()
{
    std::vector<std::string> Names = { "msft" , "appl", "appl" ,"msft", "appl" ,"msft" };
    int n = 6;
    std::string mode;

    mode = More_repeated(Names, n);
    std::cout << mode;
}
