# pharo-wars

## Pair of gloves

Winter is coming, you must prepare your ski holidays. The objective of this kata is to determine the number of pair of gloves you can constitute from the gloves you have in your drawer.

Given an array describing the color of each glove, return the number of pairs you can constitute, assuming that only gloves of the same color can form pairs.

#### Tests:

```js
input = ["red", "green", "red", "blue", "blue"]
result = 2 (1 red pair + 1 blue pair)

input = ["red", "red", "red", "red", "red", "red"]
result = 3 (3 red pairs)

input = ['red','red'] 
result = 1 
          
input = ['red','green','blue'] 
result = 0 

input = ['gray','black','purple','purple','gray','black'] 
result = 3 
```


## Two to One

Take 2 strings s1 and s2 including only letters from ato z. Return a new sorted string, the longest possible, containing distinct letters - each taken only once - coming from s1 or s2.

#### Tests:

```js
a = "xyaabbbccccdefww"
b = "xxxxyyyyabklmopq"
longest(a, b) -> "abcdefklmopqwxy"

a = "abcdefghijklmnopqrstuvwxyz"
longest(a, a) -> "abcdefghijklmnopqrstuvwxyz"

longest("aretheyhere", "yestheyarehere") -> "aehrsty" 
longest("loopingisfunbutdangerous", "lessdangerousthancoding") -> "abcdefghilnoprstu"
longest("inmanylanguages", "theresapairoffunctions") -> "acefghilmnoprstuy" 
```

## Sums of Parts

Let us consider this example (array written in general format):

ls = [0, 1, 3, 6, 10]

Its following parts:

```js
ls = [0, 1, 3, 6, 10]
ls = [1, 3, 6, 10]
ls = [3, 6, 10]
ls = [6, 10]
ls = [10]
ls = []
```

The corresponding sums are (put together in a list): [20, 20, 19, 16, 10, 0]

The function parts_sums (or its variants in other languages) will take as parameter a list ls and return a list of the sums of its parts as defined above.

#### Tests:

```js
ls = [1, 2, 3, 4, 5, 6] 
parts_sums(ls) -> [21, 20, 18, 15, 11, 6, 0]

ls = [744125, 935, 407, 454, 430, 90, 144, 6710213, 889, 810, 2579358]
parts_sums(ls) -> [10037855, 9293730, 9292795, 9292388, 9291934, 9291504, 9291414, 9291270, 2581057, 2580168, 2579358, 0]
```

## Spoonerize Me

A spoonerism is a spoken phrase in which the first letters of two of the words are swapped around, often with amusing results.

In its most basic form a spoonerism is a two word phrase in which only the first letters of each word are swapped:

"not picking" --> "pot nicking"

Your task is to create a function that takes a string of two words, separated by a space: words and returns a spoonerism of those words in a string, as in the above example.

NOTE: All input strings will contain only two words. Spoonerisms can be more complex. For example, three-word phrases in which the first letters of the first and last words are swapped: "pack of lies" --> "lack of pies" or more than one letter from a word is swapped: "flat battery --> "bat flattery" You are NOT expected to account for these, or any other nuances involved in spoonerisms.

#### Tests:

```js
spoonerize("nit picking") -> "pit nicking" ;
spoonerize("wedding bells") -> "bedding wells";
spoonerize("jelly beans") -> "belly jeans";
```

## Sum of Intervals

Write a function called sumIntervals/sum_intervals() that accepts an array of intervals, and returns the sum of all the interval lengths. Overlapping intervals should only be counted once.

Intervals
Intervals are represented by a pair of integers in the form of an array. The first value of the interval will always be less than the second value. Interval example: [1, 5] is an interval from 1 to 5. The length of this interval is 4.

Overlapping Intervals
List containing overlapping intervals:

[
   [1,4],
   [7, 10],
   [3, 5]
]

The sum of the lengths of these intervals is 7. Since [1, 4] and [3, 5] overlap, we can treat the interval as [1, 5], which has a length of 4.


#### Tests:

```js
sumIntervals( [
   [1,2],
   [6, 10],
   [11, 15]
] ); // => 9

sumIntervals( [
   [1,4],
   [7, 10],
   [3, 5]
] ); // => 7

sumIntervals( [
   [1,5],
   [10, 20],
   [1, 6],
   [16, 19],
   [5, 11]
] ); // => 19
```

## Union of Intervals

Union of closed disjoint intervals
Write a function interval_insert which takes as input

  - a list myl of disjoint closed intervals with integer endpoints, sorted by increasing order of left endpoints
  - an interval interval
  
and returns the union of interval with the intervals in myl, as an array of disjoint closed intervals.

Terminology

A closed interval includes its endpoints. For example [0,5] means greater than or equal to 0 and less than or equal to 5. For more, refer to Wikipedia.

Two intervals are said to be disjoint if they have no element in common. Equivalently, disjoint intervals are intervals whose intersection is the empty interval. For example,
[1,3] and [4,6] are disjoint
[1,3] and [3,5] are not.

#### Tests:

```js
[(1, 2)], (3, 4) -> [(1, 2), (3, 4)]
[(3, 4)], (1, 2) -> [(1, 2), (3, 4)]
[(1, 2), (4, 6)], (1, 4) -> [(1, 6)]
[(0, 2), (3, 6), (7, 7), (9, 12)], (1, 8) -> [(0, 8), (9, 12)]
```

## Digitize

Given a non-negative integer, return an array / a list of the individual digits in order.

Examples:

123 => [1,2,3]

1 => [1]

8675309 => [8,6,7,5,3,0,9]

#### Tests:

```js
digitize(123) -> [1,2,3]
digitize(1) -> [1]
digitize(0) -> [0]
digitize(1230) -> [1,2,3, 0]
digitize(8675309) -> [8,6,7,5,3,0,9]
```

#### Tests:

```js

```

## 

#### Tests:

```js

```
