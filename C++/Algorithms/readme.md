# Matrix Chain Multiplication using Recursion

Two matrices of size m*n and n*p when multiplied, they generate a matrix of size m*p and the number of multiplications performed are m*n*p.

Now, for a given chain of N matrices, the first partition can be done in N-1 ways. For example, sequence of matrices A, B, C and D can be grouped as (A)(BCD), (AB)(CD) or (ABC)(D) in these 3 ways. 

So a range [i, j] can be broken into two groups like {[i, i+1], [i+1, j]}, {[i, i+2], [i+2, j]}, . . . , {[i, j-1], [j-1, j]}.

Each of the groups can be further partitioned into smaller groups and we can find the total required multiplications by solving for each of the groups.
The minimum number of multiplications among all the first partitions is the required answer.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
