# SMHasher result for MurmurHash3A #

This is the dump of SMHasher test set
run on a Core i5 560M
using FNV hash function (32-bits version).

The function proves overall pretty bad,
with some serious bias flaws.
It also fails a few collisions test,
most notably Keyset 'Combination 0x8000000', and the cyclic tests.
Overall, it performs "reasonably poorly",
which makes it less than ideal, but still usable as a hash function.

# Result Log #
```
-------------------------------------------------------------------------------
--- Testing FNV (Fowler-Noll-Vo hash, 32-bit)

[[[ Speed Tests ]]]

Bulk speed test - 262144-byte keys
Alignment  0 -  0.228 bytes/cycle -  653.38 MiB/sec @ 3 ghz
Alignment  1 -  0.232 bytes/cycle -  663.15 MiB/sec @ 3 ghz
Alignment  2 -  0.232 bytes/cycle -  662.48 MiB/sec @ 3 ghz
Alignment  3 -  0.229 bytes/cycle -  655.20 MiB/sec @ 3 ghz
Alignment  4 -  0.232 bytes/cycle -  663.35 MiB/sec @ 3 ghz
Alignment  5 -  0.232 bytes/cycle -  663.18 MiB/sec @ 3 ghz
Alignment  6 -  0.240 bytes/cycle -  686.60 MiB/sec @ 3 ghz
Alignment  7 -  0.232 bytes/cycle -  662.63 MiB/sec @ 3 ghz

Small key speed test -    1-byte keys -    39.11 cycles/hash
Small key speed test -    2-byte keys -    32.14 cycles/hash
Small key speed test -    3-byte keys -    31.75 cycles/hash
Small key speed test -    4-byte keys -    37.21 cycles/hash
Small key speed test -    5-byte keys -    30.18 cycles/hash
Small key speed test -    6-byte keys -    34.23 cycles/hash
Small key speed test -    7-byte keys -    33.68 cycles/hash
Small key speed test -    8-byte keys -    42.47 cycles/hash
Small key speed test -    9-byte keys -    39.64 cycles/hash
Small key speed test -   10-byte keys -    37.60 cycles/hash
Small key speed test -   11-byte keys -    43.16 cycles/hash
Small key speed test -   12-byte keys -    46.11 cycles/hash
Small key speed test -   13-byte keys -    48.32 cycles/hash
Small key speed test -   14-byte keys -    50.08 cycles/hash
Small key speed test -   15-byte keys -    54.56 cycles/hash
Small key speed test -   16-byte keys -    59.82 cycles/hash
Small key speed test -   17-byte keys -    61.01 cycles/hash
Small key speed test -   18-byte keys -    66.88 cycles/hash
Small key speed test -   19-byte keys -    69.79 cycles/hash
Small key speed test -   20-byte keys -    74.82 cycles/hash
Small key speed test -   21-byte keys -    78.84 cycles/hash
Small key speed test -   22-byte keys -    84.18 cycles/hash
Small key speed test -   23-byte keys -    89.56 cycles/hash
Small key speed test -   24-byte keys -    92.28 cycles/hash
Small key speed test -   25-byte keys -    97.48 cycles/hash
Small key speed test -   26-byte keys -   106.96 cycles/hash
Small key speed test -   27-byte keys -   109.14 cycles/hash
Small key speed test -   28-byte keys -   114.58 cycles/hash
Small key speed test -   29-byte keys -   118.45 cycles/hash
Small key speed test -   30-byte keys -   126.43 cycles/hash
Small key speed test -   31-byte keys -   130.57 cycles/hash
Small key speed test -   32-byte keys -   133.71 cycles/hash

[[[ Avalanche Tests ]]]

Testing  32-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing  40-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing  48-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing  56-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing  64-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing  72-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing  80-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing  88-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing  96-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing 104-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing 112-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing 120-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing 128-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing 136-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing 144-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
Testing 152-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 100.00% !!!!! 
*********FAIL*********

[[[ Keyset 'Cyclic' Tests ]]]

Keyset 'Cyclic' - 8 cycles of 4 bytes - 10000000 keys
Testing collisions   - Expected 11641.53, actual 217246.00 (18.66x) !!!!! 
Testing distribution - Worst bias is the  20-bit window at bit   0 - 94.729% !!!!! 

Keyset 'Cyclic' - 8 cycles of 5 bytes - 10000000 keys
Testing collisions   - Expected 11641.53, actual 115440.00 ( 9.92x) !!!!! 
Testing distribution - Worst bias is the  20-bit window at bit   0 - 89.985% !!!!! 

Keyset 'Cyclic' - 8 cycles of 6 bytes - 10000000 keys
Testing collisions   - Expected 11641.53, actual 205386.00 (17.64x) !!!!! 
Testing distribution - Worst bias is the  19-bit window at bit  30 - 94.453% !!!!! 

Keyset 'Cyclic' - 8 cycles of 7 bytes - 10000000 keys
Testing collisions   - Expected 11641.53, actual 115011.00 ( 9.88x) !!!!! 
Testing distribution - Worst bias is the  20-bit window at bit  26 - 90.010% !!!!! 

Keyset 'Cyclic' - 8 cycles of 8 bytes - 10000000 keys
Testing collisions   - Expected 11641.53, actual 206223.00 (17.71x) !!!!! 
Testing distribution - Worst bias is the  20-bit window at bit  31 - 94.451% !!!!! 

*********FAIL*********

[[[ Keyset 'TwoBytes' Tests ]]]

Keyset 'TwoBytes' - up-to-4-byte keys, 652545 total keys
Testing collisions   - Expected    49.57, actual    13.00 ( 0.26x)
Testing distribution - Worst bias is the  16-bit window at bit  24 - 10.260% !!!!! 

Keyset 'TwoBytes' - up-to-8-byte keys, 5471025 total keys
Testing collisions   - Expected  3484.56, actual  7125.00 ( 2.04x) !!!!! 
Testing distribution - Worst bias is the  20-bit window at bit  22 - 1.714% !!!!! 

Keyset 'TwoBytes' - up-to-12-byte keys, 18616785 total keys
Testing collisions   - Expected 40347.77, actual 53215.00 ( 1.32x)
Testing distribution - Worst bias is the  20-bit window at bit  20 - 0.211%

Keyset 'TwoBytes' - up-to-16-byte keys, 44251425 total keys
Testing collisions   - Expected 227963.15, actual 255728.00 ( 1.12x)
Testing distribution - Worst bias is the  20-bit window at bit  19 - 0.148%

Keyset 'TwoBytes' - up-to-20-byte keys, 86536545 total keys
Testing collisions   - Expected 871784.70, actual 917142.00 ( 1.05x)
Testing distribution - Worst bias is the  20-bit window at bit  19 - 0.075%

*********FAIL*********

[[[ Keyset 'Sparse' Tests ]]]

Keyset 'Sparse' - 32-bit keys with up to 6 bits set - 1149017 keys
Testing collisions   - Expected   153.70, actual   190.00 ( 1.24x)
Testing distribution - Worst bias is the  14-bit window at bit  29 - 2.443% !!!!! 

Keyset 'Sparse' - 40-bit keys with up to 6 bits set - 4598479 keys
Testing collisions   - Expected  2461.72, actual  3619.00 ( 1.47x)
Testing distribution - Worst bias is the  19-bit window at bit  21 - 4.080% !!!!! 

Keyset 'Sparse' - 48-bit keys with up to 5 bits set - 1925357 keys
Testing collisions   - Expected   431.55, actual   481.00 ( 1.11x)
Testing distribution - Worst bias is the  17-bit window at bit  22 - 7.099% !!!!! 

Keyset 'Sparse' - 56-bit keys with up to 5 bits set - 4216423 keys
Testing collisions   - Expected  2069.66, actual  2527.00 ( 1.22x)
Testing distribution - Worst bias is the  16-bit window at bit  21 - 7.348% !!!!! 

Keyset 'Sparse' - 64-bit keys with up to 5 bits set - 8303633 keys
Testing collisions   - Expected  8026.87, actual  8745.00 ( 1.09x)
Testing distribution - Worst bias is the  20-bit window at bit   0 - 8.374% !!!!! 

Keyset 'Sparse' - 96-bit keys with up to 4 bits set - 3469497 keys
Testing collisions   - Expected  1401.34, actual  1370.00 ( 0.98x)
Testing distribution - Worst bias is the  16-bit window at bit  22 - 16.655% !!!!! 

Keyset 'Sparse' - 256-bit keys with up to 3 bits set - 2796417 keys
Testing collisions   - Expected   910.36, actual  1088.00 ( 1.20x)
Testing distribution - Worst bias is the  16-bit window at bit  22 - 32.556% !!!!! 

Keyset 'Sparse' - 2048-bit keys with up to 2 bits set - 2098177 keys
Testing collisions   - Expected   512.50, actual  1135.00 ( 2.21x) !!!!! 
Testing distribution - Worst bias is the  13-bit window at bit   0 - 56.979% !!!!! 

*********FAIL*********

[[[ Keyset 'Combination Lowbits' Tests ]]]

Keyset 'Combination' - up to 8 blocks from a set of 8 - 19173960 keys
Testing collisions   - Expected 42799.01, actual     0.00 ( 0.00x)
Testing distribution - Worst bias is the  20-bit window at bit  20 - 50.342% !!!!! 


[[[ Keyset 'Combination Highbits' Tests ]]]

Keyset 'Combination' - up to 8 blocks from a set of 8 - 19173960 keys
Testing collisions   - Expected 42799.01, actual 550392.00 (12.86x) !!!!! 
Testing distribution - Worst bias is the  19-bit window at bit  29 - 96.143% !!!!! 

*********FAIL*********

[[[ Keyset 'Combination 0x8000000' Tests ]]]

Keyset 'Combination' - up to 20 blocks from a set of 2 - 2097150 keys
Testing collisions   - Expected   512.00, actual 25340.00 (49.49x) !!!!! 
Testing distribution - Worst bias is the  18-bit window at bit   0 - 97.974% !!!!! 

*********FAIL*********

[[[ Keyset 'Combination 0x0000001' Tests ]]]

Keyset 'Combination' - up to 20 blocks from a set of 2 - 2097150 keys
Testing collisions   - Expected   512.00, actual  2768.00 ( 5.41x) !!!!! 
Testing distribution - Worst bias is the  18-bit window at bit  26 - 89.488% !!!!! 

*********FAIL*********

[[[ Keyset 'Combination Hi-Lo' Tests ]]]

Keyset 'Combination' - up to 6 blocks from a set of 15 - 12204240 keys
Testing collisions   - Expected 17339.30, actual 38790.00 ( 2.24x) !!!!! 
Testing distribution - Worst bias is the  20-bit window at bit  18 - 51.163% !!!!! 

*********FAIL*********

[[[ Keyset 'Window' Tests ]]]

Keyset 'Windowed' -  64-bit key,  20-bit window - 64 tests, 1048576 keys per test
Window at   0 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at   1 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at   2 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at   3 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at   4 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at   5 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at   6 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at   7 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at   8 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at   9 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  10 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  11 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  12 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  13 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  14 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  15 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  16 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  17 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  18 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  19 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  20 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  21 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  22 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  23 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  24 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  25 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  26 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  27 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  28 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  29 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  30 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  31 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  32 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  33 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  34 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  35 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  36 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  37 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  38 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  39 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  40 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  41 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  42 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  43 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  44 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  45 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  46 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  47 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  48 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  49 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  50 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  51 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  52 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  53 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  54 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  55 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  56 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  57 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  58 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  59 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  60 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  61 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  62 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  63 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)
Window at  64 - Testing collisions   - Expected   128.00, actual     0.00 ( 0.00x)

[[[ Keyset 'Zeroes' Tests ]]]

Keyset 'Zeroes' - 65536 keys
Testing collisions   - Expected     0.50, actual     0.00 ( 0.00x)
Testing distribution - Worst bias is the  10-bit window at bit  25 - 74.999% !!!!! 


[[[ Keyset 'Seed' Tests ]]]

Keyset 'Seed' - 1000000 keys
Testing collisions   - Expected   116.42, actual     0.00 ( 0.00x)
Testing distribution - Worst bias is the  17-bit window at bit   7 - 6.747% !!!!! 



Input vcode 0x385455b6, Output vcode 0x3f3f2ad4, Result vcode 0x00000001
Verification value is 0x00000001 - Testing took 465.320000 seconds
-------------------------------------------------------------------------------
```