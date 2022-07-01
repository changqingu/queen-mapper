# queen-mapper
queen: An excellent FPGA Technology Mapper for both Area and Performance.

### queen Vs. ABC-if

### area-oriented mapping for K = 6
#### benchmark: EPFL

The circuits have been optimized by "resyn, resyn2" scripts of ABC before mapping. 

| Benchmark name | Inputs | Outputs | ABC-if | queen | ratio |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| Adder | 256  | 129  | 249 | 192 | -23% |
| Barrel shifter | 135 | 128 | 512 | 512 | 0% | 
| Divisor  | 128 | 128 | 8205 | 6621 | -19% |
|  Hypotenuse  |  256  | 128 | 47385 | 44148 | -7% |
|  Log2  |  32  | 32  | 7709 | 6655 | -14% |
|  Max  |  512  | 130  | 724 | 736 | 2% |
|  Multiplier  |  128  | 128  | 5689 | 4595 | -19% |
|  Sine  |  24  | 25  | 1455 | 1309 | -10% |
|  Square-root  |  128  | 64  | 5054 | 3394 | -33% |
|  Square  | 64  | 128  | 3919 | 3476 | -11% |
|  Round-robin arbiter  |  256   |  129   | 2599 | 2595 | 0% |  
|  Alu control unit   |  7  | 26   | 29 | 28 | -3% |
|  Coding-cavlc    |  10  | 11   | 118 | 119 | 1% |
|  Decoder  | 8  | 256   | 287 | 288 | 0% |
|  I2c controller  |  147  | 142  | 309 | 296 | -4% |
|  Int to float converter |  11  | 7  | 46 | 45 | -2% |
|  Memory controller  |  1204  | 1231  | 11448 | 11172 | -2% |
|  Priority encoder  |  128  | 8  | 216 | 174 | -19% |
|  Lookahead XY router | 60 |30 | 74 | 48 | -35% |
|  Voter | 1001 | 1 | 1940 | 1607 | -17% |

#### Note: queen can be obtained by an ABC commmand "queen" contained in the bin/abc.
#### Contact me for bug report: changqingfans@gmail.com
