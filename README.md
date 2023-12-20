# python-quizes

# Python Quiz 1{Individual}
1. Ask a user to input their name, age, and weight in
pounds.
2. After they do convert the weight entered into pounds.

#  Python Quiz 2{Groups of 5}
Task description
Create a component that displays chips, with the ability to specify the
maximum number of displayed chips and the maximum text length in a
chip.
Introduction
Given a component called ChipList which accepts three parameters:
1. chips: the array of chips (optional);
2. maxChips: the maximum number of chips displayed (optional);
3. maxTextLength: the maximum length of text in a chip (optional);
write logic to display the component according to the requirements
specified below.
RequirementsDisplay the array of chips (the chips parameter) passed to the component
according to the following rules:
1. The number of displayed chips should be controlled by the maxChips
parameter.
2. If the maximum number of chips to be displayed is exceeded,
indicate the number of chips that are not shown in the aside element
with data-testid="exceeding-text".
3. The length of text in each chip should be controlled by the
maxTextLength parameter.
4. If the maximum length of text in a chip is exceeded, attach an ellipsis
symbol (…) after the last allowed letter.
5. If no parameters are passed or the chips array is empty, return an
empty React Fragment.
6. Handle the edge cases of:
○ no data being passed to the component;
○ an empty chips array;
○ the chips, maxChips and maxTextLength parameters being
provided in all possible configurations;
○ the maxChips and maxTextLength parameters having values
less than or equal to 0.
7. Do not change the way the App and ChipList components are
exported.8. ChipList is the component that will be tested against a set of Unit
Tests. The App component is only used for simulating the behaviour
in the Preview tab; it will be not used in the Unit Tests.
9. Ensure that the chips are displayed in the same order as they appear
in the chips property. Be sure to provide the correct index for each
chip in the data-testid property.
Assumptions
● Components and styles will be prepared upfront; your only task is to
focus on the logic to handle the parameters.
● Try not to alter the existing components, or some tests might fail.
● The maxChips and maxTextLength parameters can be either a
number or undefined.
● The chips list can be undefined, an empty array or a non-empty array.
Hints
● Show the exceeding "n more items" label only if the number of chips
is greater than the maximum quantity of chips allowed to be
displayed. There is no need to display "0 more items". Be sure not to
render the <aside> tag if there is no need to display the label.
● If the maxTextLength property is less than 1, assume that all chips
will only show the ellipsis symbol.
● If the maxChips property is less than 1, assume that only the {n}
more items label will be displayed.● Use the Preview tab to visually check the correctness of your code.
● Use the browser's developer tools in the Preview tab to debug your
code (console.log).
Available packages/libraries
● React version 18.2.0
Examples
Given a list
const sampleChips = [
{ label: "123456" },
{ label: "1234567" },
{ label: "12345678" },
{ label: "12345" },
{ label: "123456789" }
];
and calling the <ChipList /> component with the following properties:
<ChipList
chips={chips}
maxChipsDisplayed={3}
maxTextLength={6}
/>the displayed content should appear as follows:
123456 123456 123456 2 more items

# Python Quiz 3{Groups of 4}
In an even word, each letter occurs an even number of times.
Write a function solution that, given a string S consisting of N
characters, returns the minimum number of letters that must be
deleted to obtain an even word.
Examples:
1. Given S = "acbcbba", the function should return 1 (one letter b
must be deleted).
2. Given S = "axxaxa", your function should return 2 (one letter a
and one letter x must be deleted).You are given a non-empty string S consisting of N characters. In
this problem we consider only strings that consist of lower-case
English letters (a−z) and spaces. S can be divided into words by
splitting it at the spaces and removing them. We want to reverse
every word in S. For example, given S = "we test coders", there
are three words: "we", "test" and "coders". Reversing the words
gives "ew", "tset" and "sredoc". The goal is to return a string with
every word in string S reversed and separated by spaces, so the
result in the above example should be "ew tset sredoc". You can
assume that if there are K spaces in S then there are exactly K +
1 words. Write a function: def solution(S) that, given a
non-empty string S consisting of N characters, returns the
reversal of every word of S. For example, given S = "we test
coders", the function should return "ew tset sredoc", as explained
above. Write an efficient algorithm for the following
assumptions: the length of string S is within the range[1..200,000]; string S consists only of lower-case letters (a−z)
and spaces. Task idea contributed by Stephen Law of Electrum.
3. Given S = "aaaa", your function should return 0 (there is no
need to delete any letters).
Write an efficient algorithm for the following assumptions:
● N is an integer within the range [0..200,000];
● string S is made only of lowercase letters (a−z)

# Python Quiz 4{Groups of 3}
You are given a non-empty string S consisting of N characters. In this
problem we consider only strings that consist of lower-case English letters
(a−z) and spaces.
S can be divided into words by splitting it at the spaces and removing
them. We want to reverse every word in S.
For example, given S = "we test coders", there are three words: "we", "test"
and "coders". Reversing the words gives "ew", "tset" and "sredoc".The goal is to return a string with every word in string S reversed and
separated by spaces, so the result in the above example should be "ew tset
sredoc". You can assume that if there are K spaces in S then there are
exactly K + 1 words.
Write a function:
def solution(S)
that, given a non-empty string S consisting of N characters, returns the
reversal of every word of S.
For example, given S = "we test coders", the function should return "ew tset
sredoc", as explained above.
Write an efficient algorithm for the following assumptions:
● the length of string S is within the range [1..200,000];
● string S consists only of lower-case letters (a−z) and
spaces.
Task idea contributed by Stephen Law of Electrum.

# Python Quiz 5{Groups of 6}
There are N blocks, numbered from 0 to N-1, arranged in a row. A
couple of frogs were sitting together on one block when they had a
terrible quarrel. Now they want to jump away from one another so that
the distance between them will be as large as possible. The distance
between blocks numbered J and K, where J ≤ K, is computed as K − J +
1. The frogs can only jump up, meaning that they can move from one
block to another only if the two blocks are adjacent and the second
block is of the same or greater height as the first. What is the longest
distance that they can possibly create between each other, if they also
chose to sit on the optimal starting block initially?
Write a function:
def solution(blocks)
that, given an array blocks consisting of N integers denoting the
heights of the blocks, returns the longest possible distance that two
frogs can make between each other starting from one of the blocks.Examples:
1. Given blocks = [2, 6, 8, 5], the function should return 3. If starting
from blocks[0], the first frog can stay where it is and the second frog
can jump to blocks[2] (but not to blocks[3]).
2. Given blocks = [1, 5, 5, 2, 6], the function should return 4. If starting
from blocks[3], the first frog can jump to blocks[1], but not blocks[0],
and the second frog can jump to blocks[4].
3. Given blocks = [1, 1], the function should return 2. If starting from
blocks[1], the first frog can jump to blocks[0] and the second frog canstay where it is. Starting from blocks[0] would result in the same
distance.
Write an efficient algorithm for the following assumptions:
● N is an integer within the range [2..200,000];
● each element of array blocks is an integer within the
range [1..1,000,000,000].