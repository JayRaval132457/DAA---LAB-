#include <iostream>
#include <algorithm>
using namespace std;

int main()
{
    int n = 5;
    int W = 9;

    int weight[] = {5, 4, 2, 3, 6};
    int value[] = {10, 11, 2, 3, 9};

    int dp[6][10] = {0};

    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= W; j++)
        {
            if (weight[i - 1] <= j)
            {
                dp[i][j] = max(
                    dp[i - 1][j],
                    dp[i - 1][j - weight[i - 1]] + value[i - 1]
                );
            }
            else
            {
                dp[i][j] = dp[i - 1][j];
            }
        }
    }

    cout << "Maximum Value = " << dp[n][W];

    return 0;
}
