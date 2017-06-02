# Randged XORs

## Problem statement:

The first line contains two integers `N` and `Q`. 
The second line contains an array `A` with `N` integers.
Then `Q` lines follow with each 3 integers `t`, `x` and `y`.
If `t` is 1, then update `A[x]` to the value `y`. 
If `t` is 2, then print the result of `A[x] xor A[x+1] xor ... xor A[y]`. 

## Example test case:

    Input:
    5 6
    6 5 6 2 2
    2 2 3
    1 3 4
    1 1 8
    2 2 4
    1 2 0
    2 1 3

    Output:
    4
    0
    12

### Explanation:

At the beginning the array is `[6, 5, 6, 2, 2]`. 

For the first query we have to compute `A[2] xor A[3] = 6 xor 2 = 4`. 

The second query changes the array to `[6, 5, 6, 4, 2]`. 

The third query changes the array to `[6, 8, 6, 4, 2]`. 

For the fourth query we compute `A[2] xor A[3] xor A[4] = 6 xor 4 xor 2 = 0`. 

The fifth query changes the array to `[6, 8, 0, 4, 2]`. 

And for the sixth query we compute `A[1] xor A[2] xor A[3] = 8 xor 0 xor 4 = 12`. 

## More test cases:

You can generate more test cases using this [script](https://tio.run/##jZI9b4MwEIZ3fsWJyVZdhOmGSvcOococ0QoJ0lKBsYzph6L8dnqHgYS0UspiYT/3vCf79Ld9a9XdMFSNbo0Fk6uibTxPm0pZ5j8q3dvY514qYCtgAwk0uWZ4JqCiM8aDTtcVrnyuORzhcPSDfWua3DIqxLPcGKzdOX1AC7EhKjkgCS@oo/DXkqU8m1XgB@9tpRhldtYIQA1Hm2fKrq9tR8rMu6jf8tgD/Ko9XMRJARGHJAHpiJEqvtDyu6/0VvIFUuXnn9DmhGBnO3RlyCG9bJ/fyfm1YCtIC2K5k5R1V67aktf7Qir6B7V3uoeRP2XMOWL20DL@yKv9T5wr5ausFO5BhmG4DsIXw4RwtUcP95HX9HTT9cmYfDcyWxfPgueE@EsvTUKQa12qguEvX6b3qbfT@FISCWhIXIELcCAVDUMUgpRj5z8). 
