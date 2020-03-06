# max_sub_array

An implementation of max sub-array. I wrote the greedy impl but implemented the divide and conquer version referencing the pseudo algorithmn in "Introduction to Algorithms" by Cormen et al. Although the greedy algorithmn is n^2 and the divide and conquer logarithmic the greedy version performs better for the sample test case (taken from the book).

```
===============================================================================
   Name (baseline is *)   |   Dim   |  Total ms |  ns/op  |Baseline| Ops/second
===============================================================================
       benchmark_greedy * |       8 |     0.004 |     522 |      - |  1912960.3
    benchmark_logarithmic |       8 |     0.006 |     695 |  1.331 |  1437039.7
       benchmark_greedy * |      64 |     0.033 |     512 |      - |  1950268.2
    benchmark_logarithmic |      64 |     0.044 |     686 |  1.340 |  1455769.6
       benchmark_greedy * |     512 |     0.286 |     559 |      - |  1787303.9
    benchmark_logarithmic |     512 |     0.360 |     703 |  1.258 |  1420785.7
       benchmark_greedy * |    4096 |     2.377 |     580 |      - |  1722842.0
    benchmark_logarithmic |    4096 |     2.957 |     721 |  1.244 |  1385275.8
       benchmark_greedy * |    8192 |     4.602 |     561 |      - |  1780156.0
    benchmark_logarithmic |    8192 |     6.147 |     750 |  1.336 |  1332608.9
===============================================================================
```
