# Recursion

#include <iostream>

using namespace std;

int allSums(unsigned int x) 
{
    // base case
    if (x == 1) 
    {
        return x;
    }
    // recurse
    else 
    {
        return x + allSums(x - 1);
    }
}

int main()
{
    int num;
    cout << "give me a number:  " << endl;
    cin >> num;
    
    unsigned int ans = allSums(num);
    cout << ans << endl;
    
    return 0;
}
