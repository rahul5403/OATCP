Read the size of the grid, n.

Initialize a matrix dp of size (n+1) x (n+1) with all elements set to 0.

Set dp[0][0] = 1.

Loop over each cell (i, j) in the grid:

a. Read the character s[j] for each row i.

b. If s[j] is not '', update dp[i][j] by adding dp[i-1][j] and dp[i][j-1], taking modulo 1e9+7.

c. If s[j] is '', set dp[i][j] to 0.

Output dp[n-1][n-1] % (1e9+7) if n > 0, else output -1.
