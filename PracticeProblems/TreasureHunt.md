# Treasure Hunt
For this problem, you will be given a starting array called `Locations` which will serve as the input. Based on the position of each individual digit of each number, your program should decide if the number should remain as is or if it should be changed to an `X`.

### Details
Any digit that is greater than all adjacent digits should be replaced with an X. For example, if the array you were given had the locations of 111, 343, & 222, your treasure map would be setup as follows:
```
111
343
222
```
Only the 4 in 343 would be replaced with an X because it is the only digit in any of the locations that has another digit on all 4 sides AND is larger than all of its adjacent digits.
So, the output would be:
```
111
3X3
222
```

### Sample Inputs & Outputs
Input:
```CSharp
int[] Locations = {1234, 7396, 4578, 8125};
```

Outputs:
```CSharp
1234
73X6
4578
8125
```

Your program should print to the console the locations with the X's replacing the correct digits one per line. 

### Getting Started
Clone the [TreasureHunt](https://github.com/WeCanCodeIT/TreasureHunt) repository. The array `Locations` will already be included in your solution.
