# KenoBet

**Wellcome to KenoBet Project**
Kenobet is a luck game, you have to pick n  numbers in range [0,15) and your pick have to in the range (1 ,80), place a bet that will
be split in n bets rounds, it depends how much hits You get a reward.

# Run

**Step 1: Make ./keno**

```
$ g++ -Wall -std=c++11 src/main.cpp src/bet.cpp -I src/ -g
```
**Step 2: make a bet.dat "a bet file"**

vim bet.dat
1500 `Cash`
3 N `Rounds`
20 15 46 `You bets on range [0 80)`

**Step 3: Run ./keno**

```
$ ./keno data/bet.dat
```
`Dont forgot the place "Bet FILE"`

**Step 4: Game Running**

Press `Enter`
To pass rounds
To continue play
press `1` and set a `New Bet FIle`

# Error

==4332== Invalid read of size 1
==4332== at 0x4C32D32: __strlen_sse2 (in /usr/lib/valgrind/vgpreload_memcheck-amd64-linux.so)
==4332== by 0x4F61C93: std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::operator=(char const*) (in /usr/lib/x86_64-linux-gnu/libstdc++.so.6.0.25)
==4332== by 0x1099F3: main (main.cpp:14)
==4332== Address 0x0 is not stack'd, malloc'd or (recently) free'd
Error convert in=argv[i]

# Author
    **Bergony Bandeira**

`Date 12/10/2018`
