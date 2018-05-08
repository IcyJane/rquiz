# rquiz
Q1. What is the output of the below code?
a=1:2
b=1:4
a+b
A. [1] 2 4 3 4
B. [1] 2 4 4 6
C. [1] 2 4
D. [1] 1 2 1 2 3 4

Q2. What is the output of the below code?
a=data.frame(a1=1,a2=NaN,a3=NA,a4=0/0,a5=TRUE)
apply(a,2,is.nan)
A.    
   a1    a2    a3    a4    a5 
FALSE  TRUE FALSE  FALSE FALSE
B.
   a1    a2    a3    a4    a5 
FALSE  TRUE FALSE  TRUE FALSE
C.
   a1    a2   a3    a4    a5 
FALSE  TRUE TRUE  TRUE FALSE
D.    
   a1    a2    a3   a4    a5 
FALSE  TRUE TRUE  TRUE FALSE

Q3. What would be the output of the following code?
m <- matrix(1:4, nrow = 2, ncol = 2)
dimnames(m) <- list(c("a", "b"), c("c", "d"))
m
A.
  c d
a 1 3
b 2 4
B.
  c d
a 1 2
b 3 4 
C.
  a b
c 1 3
d 2 4
D.
  a b
c 1 2
d 3 4 

Q4. What is the output of the below code?
x <- c("a", "b", "c", "c", "d", "a")
x[c(1, 3, 9)]
A. [1] "a" "c" NA 
B. [1] "a" "c"
C. [1] "a" "c" "c"
D. [1] "b" "c" NA 

Q5. What is the output of the below code?
x <- matrix(1:6, 2, 3)
x[1, 2]
A. 3
B. 2
C. 4
D. None of above.

Q6.Which of the following code extracts the first element of the element b in list?
x <- list(a = list(1, 2, 4), b = c(6, 8))
A. x[[c(2, 1)]]
B. x[[2]][1]
C. x$b[1]
D. All of the above.

Q7. What is the output of the below code?
x <- c(1,2,1,0,0,1,3, NA, NaN)
ifelse(x > 1, 1, 0)
A. [1]  0  1  0  0  0  0  1 NA NA
B. [1]  0  1  0  0  0  0  1  0  0
C. [1]  0  1  0  0  0  0  1  1  1
D. None of above.

Q8.What is the output of the below code?
x <- c(1,2,1,0,0,1,3, NA, NaN)
which(x < 1)
A. [1] 4 5
B. [1] 4 5 8 9
C. [1] FALSE  FALSE  FALSE  TRUE  TRUE  FALSE  FALSE  FALSE  FALSE 
D. [1] FALSE  FALSE  FALSE  TRUE  TRUE  FALSE  FALSE  TRUE  TRUE  

Q9.What is the output of the below code?
x <- c(1,2,1,0,0,1,3, NA, NaN)
ifelse(x %in% c(1,2), 1, 0)
A. [1]  1 1 1 0 0 1 0 0 0
B. [1]  1 1 1 0 0 1 0 NA NA
C. [1]  1 1 1 0 0 1 0 1 1
D. None of above.

Q10.
Which of the following codes can read the above csv with 3 rows into a dataframe? 
A. dataframe1=read.csv(‘Dataframe.csv’)
B. dataframe1==read.csv(‘Dataframe.csv’,header=TRUE)
C. dataframe1=dataframe(‘Dataframe.csv’)
D. dataframe1==read.csv2(‘Dataframe.csv’,header=FALSE,sep=’,’)
Answer: D

Q11.
Which of the following codes will read the above data in the third sheet into a dataframe?
A.
library(openxlsx)
dataframe1=read.xlsx(“Data.xlsx”,sheet=3,colNames=FALSE)
B. 
library(xlsx)	
dataframe1=read.xlsx(“Data.xlsx”,sheetIndex=3,header=FALSE)
C. 
library(xlConnect)
dataframe1=readWorksheetFromFile(“Data.xlsx”,sheet=3,header=FALSE)
D. All of the above
Answer: D

Q12.
Which of the following codes will not give the number of missing values in each column?
A. colSums(is.na(dataframe))
B. apply(is.na(dataframe),2,sum)
C. sapply(dataframe,function(x) sum(is.na(x)))
D. table(is.na(dataframe))
Solution: (D)

Q13.
Which of the following code will select only the rows for which Group is Group1?
A. subset(dataframe, Group ='Group1’)
B. subset(dataframe, Group =='Group1’)
C. filter(dataframe, Group =='Group1’)
D. Both B and C
E. All of the above

Q14.
Which of the following commands will produce the desired output?
A) format(df,”%d %A %b %y”)
B) format(df,”%D %A %b %y”)
C) format(df,”%D %a %B %Y”)
D) None of above


Q16.
Please define a function that counts the number of subsrings that match the following pattern: "a?b" where "?" can be any single character.
e.g. f("dasbragbgh")=2
Q17.
Please define a function that counts the number of substrings that contain 2 consecutive characters.
e.g f("yefguio")=2 
Q18.
Please define a function that counts the number of substrings that contain consecutive characters.
e.g f("yefguiabo")=2, i.e. "efg" and "ab"
Q19.
Please define a function that calculates the score rank for each person in his/her team.
Q20.
Please define a function that calculates the number of people of opposing gender in their own team he/she exceeds in terms of score.
Q21.
Please define a function that calculates the number of pairs (two people) in which the older person has a lower score.
