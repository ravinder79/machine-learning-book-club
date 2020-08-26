# Introduction to Applied Linear Algebra - Vectors, Matrices, and Least Squares

## Chapter 1: Vectors

### Exercise solutions:

#### Exercise 1:

a. True and valid notation\
b. Not a valid notation\
c. Valid notation and true (stacked vector)

#### Exercise 2:

a. correct notation - same size vectors of addition/subtraction\
b. correct notation - stacked vectors\
c. incorrect notation - different sized vectors (10 vs 20)\
d. correct notation\
e. correct notation\
f. incorect notation\
g. correct notation

#### Exercise 3:

a. correct notation and unambigous\
b. correct notation but invalid (different size)
c. correct but ambigous\
d. valid notation but incorrect


#### Exercise 4: Periodic energy usage.

a. w = (d,d,d,d,d,d,d)\
b. d = w<sub>1:24</sub>



#### Exercise 5: Interpreting sparsity  

(a) x represents the daily cash flow of some business over n days: 
 ***Zero cashflow on most days of the business***  
(b) x represents the annual dollar value purchases by a customer of n products or services: ***Customer did not spend on most products or services in that year.***  
(c) x represents a portfolio, say, the dollar value holdings of n stocks: ***portfolio contains only a few of n stocks***  
(d) x represents a bill of materials for a project, i.e., the amounts of n materials needed: *** project requires only few of the n materials***.  
(e) x represents a monochrome image, i.e., the brightness values of n pixels: ***the image is mostly dark e.g. imaging a dark sky with few distant stars/galaxies***  
(f) x is the daily rainfall in a location over one year. ***how it feels like living in death valley***    

  

#### Exercise 6: Vector of differences.  

x<sub>2:n</sub> - x<sub>1:n-1</sub>

#### Exercise 7: Transforming between two encodings for Boolean vectors.
x = (1,0,0, 1,) ---> (+1, -1, -1, +1)

y = 2x -1 

x = (y+1) * 1/2


#### Exercise 8: Profit and sales vectors.
p is profit/loss per item  
s is sales for each item  

Total profit is inner product of p and s  
p<sup>T</sup>s


#### Exercise 9: Symptoms vector  
***Inner product   (Page 20)***   
•  Unit vector. eTi a = ai. The inner product of a vector with the ith standard unit vector gives (or ‘picks out’) the ith element a.  
• Sum. 1T a = a1 + · · · + an. The inner product of a vector with the vector of ones gives the sum of the elements of the vector.  
• Average. (1/n)Ta=(a1+···+an)/n. The inner product of an n-vector with the vector 1/n gives the average or mean of the elements of the vector. The average of the entries of a vector is denoted by avg(x). The Greek letter μ is a traditional symbol used to denote the average or mean.  
• Sum of squares. a a = a1 + ··· + an. The inner product of a vector with
itself gives the sum of the squares of the elements of the vector.  
• Selective sum. Let b be a vector all of whose entries are either 0 or 1. Then
b<sup>T</sup>a is the sum of the elements in a for which b<sub>i</sub> =1.  

a. ***Total # of symptoms***  = 1<sup>T</sup>s

b. The patient exhibits five out of the first ten symptoms. ??


#### Exercise 10: Total score from course record  
s = w<sup>T</sup>r  

change each to same scale:       
Homework weightage: 100/80   
midterm weightage = 100/120   
final exam weightage = 100/160   

Now multiply each term above by their corresponding weightage  

s = 100/80  * 0.25 (r1,r2...r8, ) + 0.35 * 100/120 * r9  +  0.40 * 100/160 * r10

w = (0.3125, 0.3125, 0.3125, 0.3125, 0.3125, 0.3125, 0.3125, 0.3125, 0.2917, 0.25)

#### Exercise 11: Word count and word count histogram vectors. 

(a) What is 1<sup>T</sup>w?  
***Total number of words (sum) in the document***  

(b) What does w282 = 0 mean?  
***Word 282 is not in the document***   

(c) w / total number of words (calculated above in a)  
***h =  w/ 1<sup>T</sup>w***

#### Exercise 12: Total cash value  
Exchange rate vector e = (e1,e2,e3,e4,e5), here e1 = 1 (USD exhange rate)  
***Total cash value = e<sup>T</sup>c***  

#### Exercise 13: Average age in a population  
(a) 1<sup>T</sup>x  
(b) 1<sup>T</sup>x<sub>66:100</sub>   
(c) average age = i<sup>T</sup>x/   1<sup>T</sup>x   
    where i = (1,2,3...100)  

#### Exercise 14: Industry or sector exposure    
 long-only portfolio portfolio means all entries are positive   
 neutral portfolio =  f<sup>T</sup> h = 0.  
 Only way this could be zero is when each entry of h is zero? no investment?
  

#### Exercise 15 Cheapest supplier  
Calculate p<sub>i</sub><sup>T</sup> q  
choose lowest value (vector notation)  

to diversify we can choose two different cheapest suppliers however, it would cost more than just choosing a single lowest supplier??

#### Exercise 16 Inner product of nonnegative vectors  

(a) product of two non-negative numbers is always non-negative. adding all non-negative number is always non-negative.  
(b) Either both the vectors are zero or one of them is zero vector.  

#### Exercise 17  Linear combinations of cash flows.  

??

#### Exercise 18 Linear combinations of linear combinations.   

b1, b2 is linear combination of vectors a1 and a2  
c is linear combination of b1 and b2  

show that c is linear combination of a1 and a2

b1 = β1*a1 + β2 * a2

b2 = β3 * a1 +  β4 * a2

c = β5 * b1 +  β6 * b2

c = β5 * (β1*a1 + β2 * a2) +  β6 * (β3 * a1 +  β4 * a2)

c = (β5 * β1 + β6 * β3  ) * a1  +  (β5 * β2) +  β6 *  β4) * a2

#### Exercise 19 Auto-regressive model

 M-vector β is the AR model coefficient vector.

 (a) β ≈ e1
 
 ***This means prediction at z<sub>t+1</sub> is equal to z<sub>t</sub>***

 (b) β ≈ 2e1 − e2.  

 **z<sub>t+1</sub> = 2 * z<sub>t</sub> - z<sub>t-1</sub>**


(c) β ≈ e6.  
  *** z<sub>t+1</sub> = prediction is same as value 6 days before***

(d) β ≈ 0.5e1 + 0.5e2

   ***z<sub>t+1</sub> = average of previous two days***  

   #### Exercise 20

How many bytes does it take to store 100 vectors of length 105?  
Storing an n-vector requires 8n bytes to store.

***8 * 100 *  10<sup>5</sup>***

How many flops does it take to form a linear combination of them (with 100 nonzero coefficients)? 

    Scalar-vector multiplication ax, where x is an n-vector, requires n multiplications, i.e., axi for i = 1, . . . , n. Vector addition x + y of two n-vectors takes n additions, i.e., xi + yi for i = 1, . . . , n.

Coeffcient multiplication with each element of a vector = 100 * 10<sup>5</sup>   
Adding 10<sup>5</sup>  elements for each of 100 vectors = 100 * 10<sup>5</sup>  

***Total flop:  100 * 10<sup>5</sup>   + 100 * 10<sup>5</sup>   =   200 * 10<sup>5</sup>***

About how long would this take on a computer capable of carrying out 1 Gflop/s?   

***Time taken*** = 200 * 10<sup>5</sup> / 1000000000 = ***0.02 secs***

