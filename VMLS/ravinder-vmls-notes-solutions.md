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
g. correct notation\

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

change each to same scale
each homework weightage: 100/80 
midterm weightage = 100/120 
final exam weightage = 100/160 
multiply by weightage

s = 100/80  * 0.25 (r1,r2...r8, ) + 0.35 * 100/120 * r9  +  0.40 * 100/160 * r10

w = (0.3125, 0.3125, 0.3125, 0.3125, 0.3125, 0.3125, 0.3125, 0.3125, 0.2917, 0.25)

#### Exercise 11: Word count and word count histogram vectors. 