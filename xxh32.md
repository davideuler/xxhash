# SMHasher result for XXH32 #

This is the dump of SMHasher test set
run on a Core i5 560M
using XXH32() function.


# Result Log #
```
-------------------------------------------------------------------------------
--- Testing xxh32 (xxHash32 -- 32-bits output)

[[[ Speed Tests ]]]

Bulk speed test - 262144-byte keys
Alignment  0 -  2.137 bytes/cycle - 6113.02 MiB/sec @ 3 ghz
Alignment  1 -  2.050 bytes/cycle - 5863.99 MiB/sec @ 3 ghz
Alignment  2 -  2.197 bytes/cycle - 6286.80 MiB/sec @ 3 ghz
Alignment  3 -  2.096 bytes/cycle - 5996.60 MiB/sec @ 3 ghz
Alignment  4 -  2.183 bytes/cycle - 6245.49 MiB/sec @ 3 ghz
Alignment  5 -  2.180 bytes/cycle - 6237.00 MiB/sec @ 3 ghz
Alignment  6 -  2.183 bytes/cycle - 6245.11 MiB/sec @ 3 ghz
Alignment  7 -  2.285 bytes/cycle - 6538.21 MiB/sec @ 3 ghz

Small key speed test -    1-byte keys -    38.69 cycles/hash
Small key speed test -    2-byte keys -    42.32 cycles/hash
Small key speed test -    3-byte keys -    37.71 cycles/hash
Small key speed test -    4-byte keys -    37.27 cycles/hash
Small key speed test -    5-byte keys -    34.15 cycles/hash
Small key speed test -    6-byte keys -    38.04 cycles/hash
Small key speed test -    7-byte keys -    36.42 cycles/hash
Small key speed test -    8-byte keys -    31.55 cycles/hash
Small key speed test -    9-byte keys -    38.67 cycles/hash
Small key speed test -   10-byte keys -    38.71 cycles/hash
Small key speed test -   11-byte keys -    39.84 cycles/hash
Small key speed test -   12-byte keys -    36.29 cycles/hash
Small key speed test -   13-byte keys -    36.56 cycles/hash
Small key speed test -   14-byte keys -    37.11 cycles/hash
Small key speed test -   15-byte keys -    41.97 cycles/hash
Small key speed test -   16-byte keys -    44.25 cycles/hash
Small key speed test -   17-byte keys -    44.52 cycles/hash
Small key speed test -   18-byte keys -    48.30 cycles/hash
Small key speed test -   19-byte keys -    48.03 cycles/hash
Small key speed test -   20-byte keys -    42.72 cycles/hash
Small key speed test -   21-byte keys -    44.93 cycles/hash
Small key speed test -   22-byte keys -    48.88 cycles/hash
Small key speed test -   23-byte keys -    54.23 cycles/hash
Small key speed test -   24-byte keys -    46.28 cycles/hash
Small key speed test -   25-byte keys -    49.70 cycles/hash
Small key speed test -   26-byte keys -    51.01 cycles/hash
Small key speed test -   27-byte keys -    56.20 cycles/hash
Small key speed test -   28-byte keys -    50.54 cycles/hash
Small key speed test -   29-byte keys -    53.46 cycles/hash
Small key speed test -   30-byte keys -    53.54 cycles/hash
Small key speed test -   31-byte keys -    57.09 cycles/hash
Small key speed test -   32-byte keys -    50.02 cycles/hash

[[[ Avalanche Tests ]]]

Testing  32-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.61%
Testing  40-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.63%
Testing  48-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.56%
Testing  56-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.65%
Testing  64-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.72%
Testing  72-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.67%
Testing  80-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.71%
Testing  88-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.65%
Testing  96-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.70%
Testing 104-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.66%
Testing 112-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.80%
Testing 120-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.62%
Testing 128-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.73%
Testing 136-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.64%
Testing 144-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.73%
Testing 152-bit keys ->  32-bit hashes,   300000 reps.......... worst bias is 0.67%

[[[ Keyset 'Cyclic' Tests ]]]

Keyset 'Cyclic' - 8 cycles of 4 bytes - 10000000 keys
Testing collisions   - Expected 11641.53, actual 13288.00 ( 1.14x)
Testing distribution - Worst bias is the  20-bit window at bit  15 - 0.027%

Keyset 'Cyclic' - 8 cycles of 5 bytes - 10000000 keys
Testing collisions   - Expected 11641.53, actual 11648.00 ( 1.00x)
Testing distribution - Worst bias is the  20-bit window at bit  27 - 0.024%

Keyset 'Cyclic' - 8 cycles of 6 bytes - 10000000 keys
Testing collisions   - Expected 11641.53, actual 11818.00 ( 1.02x)
Testing distribution - Worst bias is the  20-bit window at bit   0 - 0.047%

Keyset 'Cyclic' - 8 cycles of 7 bytes - 10000000 keys
Testing collisions   - Expected 11641.53, actual 11775.00 ( 1.01x)
Testing distribution - Worst bias is the  20-bit window at bit  19 - 0.042%

Keyset 'Cyclic' - 8 cycles of 8 bytes - 10000000 keys
Testing collisions   - Expected 11641.53, actual 11698.00 ( 1.00x)
Testing distribution - Worst bias is the  20-bit window at bit   2 - 0.029%


[[[ Keyset 'TwoBytes' Tests ]]]

Keyset 'TwoBytes' - up-to-4-byte keys, 652545 total keys
Testing collisions   - Expected    49.57, actual    21.00 ( 0.42x)
Testing distribution - Worst bias is the  16-bit window at bit   4 - 0.120%

Keyset 'TwoBytes' - up-to-8-byte keys, 5471025 total keys
Testing collisions   - Expected  3484.56, actual  5704.00 ( 1.64x)
Testing distribution - Worst bias is the  20-bit window at bit  15 - 0.080%

Keyset 'TwoBytes' - up-to-12-byte keys, 18616785 total keys
Testing collisions   - Expected 40347.77, actual 54791.00 ( 1.36x)
Testing distribution - Worst bias is the  20-bit window at bit   9 - 0.031%

Keyset 'TwoBytes' - up-to-16-byte keys, 44251425 total keys
Testing collisions   - Expected 227963.15, actual 303277.00 ( 1.33x)
Testing distribution - Worst bias is the  20-bit window at bit  30 - 0.017%

Keyset 'TwoBytes' - up-to-20-byte keys, 86536545 total keys
Testing collisions   - Expected 871784.70, actual 1120225.00 ( 1.28x)
Testing distribution - Worst bias is the  20-bit window at bit   1 - 0.012%


[[[ Keyset 'Sparse' Tests ]]]

Keyset 'Sparse' - 32-bit keys with up to 6 bits set - 1149017 keys
Testing collisions   - Expected   153.70, actual     0.00 ( 0.00x)
Testing distribution - Worst bias is the  17-bit window at bit  18 - 0.136%

Keyset 'Sparse' - 40-bit keys with up to 6 bits set - 4598479 keys
Testing collisions   - Expected  2461.72, actual  1569.00 ( 0.64x)
Testing distribution - Worst bias is the  18-bit window at bit   5 - 0.026%

Keyset 'Sparse' - 48-bit keys with up to 5 bits set - 1925357 keys
Testing collisions   - Expected   431.55, actual   415.00 ( 0.96x)
Testing distribution - Worst bias is the  18-bit window at bit   2 - 0.055%

Keyset 'Sparse' - 56-bit keys with up to 5 bits set - 4216423 keys
Testing collisions   - Expected  2069.66, actual  1904.00 ( 0.92x)
Testing distribution - Worst bias is the  19-bit window at bit   2 - 0.045%

Keyset 'Sparse' - 64-bit keys with up to 5 bits set - 8303633 keys
Testing collisions   - Expected  8026.87, actual 12402.00 ( 1.55x)
Testing distribution - Worst bias is the  20-bit window at bit   1 - 0.035%

Keyset 'Sparse' - 96-bit keys with up to 4 bits set - 3469497 keys
Testing collisions   - Expected  1401.34, actual  1882.00 ( 1.34x)
Testing distribution - Worst bias is the  19-bit window at bit  13 - 0.053%

Keyset 'Sparse' - 256-bit keys with up to 3 bits set - 2796417 keys
Testing collisions   - Expected   910.36, actual   934.00 ( 1.03x)
Testing distribution - Worst bias is the  19-bit window at bit  16 - 0.069%

Keyset 'Sparse' - 2048-bit keys with up to 2 bits set - 2098177 keys
Testing collisions   - Expected   512.50, actual   499.00 ( 0.97x)
Testing distribution - Worst bias is the  18-bit window at bit  20 - 0.093%


[[[ Keyset 'Combination Lowbits' Tests ]]]

Keyset 'Combination' - up to 8 blocks from a set of 8 - 19173960 keys
Testing collisions   - Expected 42799.01, actual 39339.00 ( 0.92x)
Testing distribution - Worst bias is the  20-bit window at bit   2 - 0.027%


[[[ Keyset 'Combination Highbits' Tests ]]]

Keyset 'Combination' - up to 8 blocks from a set of 8 - 19173960 keys
Testing collisions   - Expected 42799.01, actual 52120.00 ( 1.22x)
Testing distribution - Worst bias is the  20-bit window at bit  12 - 0.027%


[[[ Keyset 'Combination 0x8000000' Tests ]]]

Keyset 'Combination' - up to 20 blocks from a set of 2 - 2097150 keys
Testing collisions   - Expected   512.00, actual   527.00 ( 1.03x)
Testing distribution - Worst bias is the  17-bit window at bit  10 - 0.041%


[[[ Keyset 'Combination 0x0000001' Tests ]]]

Keyset 'Combination' - up to 20 blocks from a set of 2 - 2097150 keys
Testing collisions   - Expected   512.00, actual   501.00 ( 0.98x)
Testing distribution - Worst bias is the  18-bit window at bit  19 - 0.064%


[[[ Keyset 'Combination Hi-Lo' Tests ]]]

Keyset 'Combination' - up to 6 blocks from a set of 15 - 12204240 keys
Testing collisions   - Expected 17339.30, actual 18655.00 ( 1.08x)
Testing distribution - Worst bias is the  20-bit window at bit  15 - 0.025%


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
Testing distribution - Worst bias is the  13-bit window at bit  27 - 0.269%


[[[ Keyset 'Seed' Tests ]]]

Keyset 'Seed' - 1000000 keys
Testing collisions   - Expected   116.42, actual    40.00 ( 0.34x)
Testing distribution - Worst bias is the  17-bit window at bit  11 - 0.080%



Input vcode 0x385455b6, Output vcode 0x0ceacd33, Result vcode 0x00000001
Verification value is 0x00000001 - Testing took 465.779000 seconds
-------------------------------------------------------------------------------
```