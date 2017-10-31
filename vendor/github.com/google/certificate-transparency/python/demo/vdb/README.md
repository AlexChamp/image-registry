IMPORTANT:
This is demo code only and not considered robust or well tested.


Play with the general purpose database demo (help works too):

```
$ python demo_general_database.py 
Type "help" to get started.
> set a 0
Value:      0
Proof:      [256]
Map hash:   nP1psZp1bu3jrY5Yv89rI+w5ywe9lLqI2qZi5ibTSF0=
Log hash:   lkr1xY8VW6cxvpGUsD2yqiTrjc0b0ODtQjuoZAe6gZM=
Tree size:  1
> dump
Tree:
H: nP1psZp1bu3jrY5Yv89rI+w5ywe9lLqI2qZi5ibTSF0=
V:'0'
P:1100101010010111100000010001001011001010000110111011110111001010111110101100001000110001101100111001101000100011110111000100110110100111100001101110111111111000000101000111110001001110011100101011100110000000011101111000010110101111111011100100100010111011
> set b 1
Value:      1
Proof:      ['daMAkHf1WBaMcAV3TG5yX2BpEJ/qBUXyhxgEY0UGTIA=', 255]
Map hash:   EJ1Rw6DQT9bDn2Zbn7u+9/j799PSdqT9gfBymS9MBZY=
Log hash:   sgshxO2oKRkhu05c/f/lszSh8q1CEz7fU8cpB8zcSFA=
Tree size:  2
> dump
Tree:
H: EJ1Rw6DQT9bDn2Zbn7u+9/j799PSdqT9gfBymS9MBZY=
L:
  H: q1BN5wwrHEONK2qXNLgp1pJh8QbeyvHlczCmEa6rphQ=
  V:'1'
  P:0011111000100011111010000001011000000000001110010101100101001010001100111000100101001111011001010110010011100001101100010011010010001011101111010111101000000000100010001101010000101100010010101100101101110011111011101010111011010101100111000000000010011101
R:
  H: daMAkHf1WBaMcAV3TG5yX2BpEJ/qBUXyhxgEY0UGTIA=
  V:'0'
  P:1100101010010111100000010001001011001010000110111011110111001010111110101100001000110001101100111001101000100011110111000100110110100111100001101110111111111000000101000111110001001110011100101011100110000000011101111000010110101111111011100100100010111011
> set a 2
Value:      2
Proof:      ['q1BN5wwrHEONK2qXNLgp1pJh8QbeyvHlczCmEa6rphQ=', 255]
Map hash:   2rAZz4HJAMJqJ5c8ClS4wEzTP71GTdjMZMe1rKWPA5o=
Log hash:   dMrfwICbRqwu6jO5bE8psiJ51j56f5U+icJzUCjN1qk=
Tree size:  3
> log
0 {"operation": "set", "value": "0", "key": "a"}
1 {"operation": "set", "value": "1", "key": "b"}
2 {"operation": "set", "value": "2", "key": "a"}
> get a 0
Value:      None
Proof:      [256]
Map hash:   xmifEIEqCYCXbZUz2Dh1KCFmFZVn7DUVVxbBQTr1PWo=
Log hash:   None
Tree size:  0
> get a 1
Value:      0
Proof:      [256]
Map hash:   nP1psZp1bu3jrY5Yv89rI+w5ywe9lLqI2qZi5ibTSF0=
Log hash:   lkr1xY8VW6cxvpGUsD2yqiTrjc0b0ODtQjuoZAe6gZM=
Tree size:  1
> get a 2
Value:      0
Proof:      ['q1BN5wwrHEONK2qXNLgp1pJh8QbeyvHlczCmEa6rphQ=', 255]
Map hash:   EJ1Rw6DQT9bDn2Zbn7u+9/j799PSdqT9gfBymS9MBZY=
Log hash:   sgshxO2oKRkhu05c/f/lszSh8q1CEz7fU8cpB8zcSFA=
Tree size:  2
> get a 3
Value:      2
Proof:      ['q1BN5wwrHEONK2qXNLgp1pJh8QbeyvHlczCmEa6rphQ=', 255]
Map hash:   2rAZz4HJAMJqJ5c8ClS4wEzTP71GTdjMZMe1rKWPA5o=
Log hash:   dMrfwICbRqwu6jO5bE8psiJ51j56f5U+icJzUCjN1qk=
Tree size:  3
> save foo
```