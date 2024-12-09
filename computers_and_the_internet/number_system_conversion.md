# binary to decimal conversion
### 8 bit example

1. take your binary number and write out the power placements underneath
    - 0    0    1    1    0    1    0    1
    - 2^7  2^6  2^5  2^4  2^3  2^2  2^1  2^0

2. calculate the powers to get the place values
    - 2^7  2^6  2^5  2^4  2^3  2^2  2^1  2^0
    - 128  64   32   16   8    4    2    1

3. multiply each bit by its place value.
    - 0    0    1    1    0    1    0    1
    - *    *    *    *    *    *    *    *
    - 128  64   32   16   8    4    2    1

4. sum up the result of each bits multiplication
    - 0  + 0  + 32 + 16 + 0  + 4  + 0  + 1
    - sum = 53
    + 53 is the decimal conversion of binary 00110101

# decimal to binary conversion
### 8 bit example

1. starting with decimal 48, you need to figure out how many bits you need.
    - 4 bits can display decimal values up to 15
    - 8 bits can display decimal values up to 255
    - we need 8 bits. so we write out place value for each binary bit we need.
    - 128  64   32   16   8    4    2    1

2. now starting from the highest value bit we check if the decimal value of our number is higher than the bit value
    - is 48 >= 128, no so we write a 0 for binary in 128's place
    - 0

3. carry over the decimal value to the next highest binary value placement
    - is 48 >= 64, no so write a 0 for binary in 64's place
    - 0    0

4. carry over to the next bit again
    - is 48 >= 32, yes
    - now that our answer is yes we can write a 1 in the 32's place of our binary
    - 0    0    1
    - the we subtract the binary place value from our decimal number
    - 48 - 32 = 16
    - now we carry over the remainder of our decimal number to the next bit

5. repeat the process until every bit is 1 or 0
    - the final output of decimal 48 in binary is
    - 0    0    1    1    0    0    0    0

# binary to hexidecimal conversion