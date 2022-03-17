
The dice game of craps is played as follows: 
1. The player rolls a pair of standard 6-sided dice and takes their sum 
   a. If the sum is 7 or 11, then the player wins and the game is over 
   b. If the sum is 2, 3, or 12, then the player loses (this is called “crapping out”) and the game is over 
   c. If the sum is anything else, then we record the sum (lets call it “X”) and continue to the next step 
2. The player then rerolls the dice and takes their sum 
   a. If the sum is X, the player wins and the game is over 
   b. If the sum is 7, the player loses and the game is over
   c. If the sum is anything else, repeat step 2. 
Now suppose that you notice something odd - one of the two dice isn’t balanced that well, and always comes up in the range 2-5 (with equal probability) but never 1 or 6.


### 1 .Probabilistic Dice Game

CODE : Taking into account the challenge and questions , several different python methods are presented for the exercise according to the following criteria:

 Generalization over probability distribution calculation in any 2 dice games.There are three methods :

   dice_prob : A function calculates the probability distribution of sum in any 2 dice games, taking as an input the range of equality distributed probability n-sided dice . The output of this function returns a dictionary defined with a key ,value pair in which the key corresponds to the different possible sums and the value corresponds to the probability distribution of each sum .
    
   Calculate_prob takes as an input the combinatorial matrix and produces the dictionary of probabilities and calculate_prob_percentages transform these probability into percentage.

   Definition of the game. A second function defines the conditions of the game and calculates the probability of winning or losing taking the second roll conditioned probability principle. The input of this function is the dice probability dictionary calculated in the first function and the result of the sum. The output is the probability of winning or losing taking into account the input.
    
The motivation under this code structure is to separate the possible game definitions from the dice truncated design and the possibility to design truncated dice that could change probability distributions over different sets of games.


KEY PROBABILITY PRINCIPLES : conditioned probability .

### 1. For each number between 2 and 12, what is the probability of rolling the dice so that they sum to that number?

The probability of rolling the dice so that they sum up to each number is described from lowest to highest and grouped in sums of the same probability : the sum of 2 and 12 is 0 . The sum of 3 and 11 have a probability of 4.1667 % . The probability of getting a sum 4 and 10 is 8.334 % and the sum of 5 and 9 has a probability of 12.5 % . Ranging from 6 to 8 there is an equal probability of 16.668 %
     
 Find above the probability of each sum in a dictionary data structure form (output of the function dice_prob )
{ 2 : 0.0 %
3 : 4,1667 %
4 : 8.334 %
5 : 12.5 %
6 : 16.668 % 7 : 16.668 % 8 : 16.668 % 9 : 12.5 %
10 : 8.334 % 11 : 4.1667 % 12 : 0 % }

For solving this question , a board exercise of matrix possibilities was drawn taking into account a 2 dice game with 6 faces and a truncated dice ranging from 2 to 5 . From there , some key concepts such as number of possibilities ( m * n ) , max sum ( m+n ) or tuples of dice faces and sum where displayed .
 

 
 ![Screenshot](https://github.com/SoyGema/Portfolio/blob/main/DataExploration/Matrix_prob_dice.png)
 
 Fig 1. Matrix Probability distribution schema comparing 2-sided dices equally distributed and game with truncated dice . Each cell gives us information about the sum in form of a tuple and the distribution for 2-sided dices equally distributed ( blue ) and truncated dice ( grey )


For calculating the probabilities , the solution proposes counting the number of repeated sums and storing it as a value inside a dictionary .


#### 2.a. What’s the probability of winning on the very first roll?


The probability of winning on the first roll according to the description of the game is 20.8336% .


#### 2.b. What’s the probability of losing (“crapping out”) on the very first roll?


The probability of crapping out on the very first roll is 4.1667 %




### 2 .Squirrels Data analysis
