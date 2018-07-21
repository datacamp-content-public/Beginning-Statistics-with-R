---
  title: "Template Chapter 1"
  description: "This is a template chapter."
---

## Recognize a statistical question

```yaml
type: PureMultipleChoiceExercise 
xp: 50 
key: 5e51bfcb9d   
```


A statistical question is a question that can be answered by collecting data. Almost all data has some variability. Variability means that repeated measurements of similar items give different numbers (the numbers vary).

A deterministic question is a question with one exact answer. The number never changes.

Example of a statistical question:
How much time do students at  my school spend on math homework each week?

Example of a deterministic question:
How many pennies are in a dime?

Abby went to the store a bought a bag of jelly beans, and has not opened it yet. Which of the following is not a statistical question about jelly beans?


`@hint`
If there is only one possible correct answer to the question, it is deterministic.
If there are multiple possible correct answers, or the correct answer could change, then it is a statistical question.

`@possible_answers`
- What is a typical number of jelly beans in a bag?
 - [How much does Abby's bag weigh?]
 - Which color is the most frequent?
 - If Abby closed her eyes, shook up the bag, reached in and grabbed a jelly bean, how likely will it be red?
 - What is the typical weight of a jelly bean?
 - How are the jelly beans distributed according to color?

`@feedbacks`
Try again

---

## Maximum and minimum values

```yaml
type: BulletExercise 
xp: 100 
key: 8fb45ad353   
```

If you type in the name of a dataset, it will print out on the screen.

* If you enter max(data), the maximum value will be returned (what is the max value).
* If you enter which.max(data), the maximum value will be returned (which one has the maximum).
* If you enter min(data), the maximum value will be returned (what is the min value).
* If you enter which.min(data), the maximum value will be returned (which one has the minimum).

The dataset Electorial_Votes is loaded for you.
* Print the Electorial_Votes dataset on the screen
* Find the largest number of electorial votes
* Find which state/district that has the most electorial votes
* Find the smallest number of electorial votes
* Find which state/district that has the fewest electorial votes

`@pre_exercise_code`

```{r}
Electorial_Votes <- matrix(c(9,3,11,6,55,9,7,3,3,29,16,4,4,20,11,6,6,8,8,4,10,11,16,10,6,10,3,5,6,4,14,5,29,15,3,18,7,7,20,4,9,3,11,38,6,3,13,12,5,10,3),ncol = 1)
rownames(Electorial_Votes) <- c(
  "Alabama","Alaska","Arizona","Arkansas","California","Colorado","Connecticut","Delaware","District of Columbia","Florida","Georgia","Hawaii","Idaho","Illinois","Indiana","Iowa","Kansas","Kentucky","Louisiana","Maine","Maryland","Massachusetts","Michigan","Minnesota","Mississippi","Missouri","Montana","Nebraska","Nevada","New Hampshire","New Jersey","New Mexico","New York","North Carolina","North Dakota","Ohio","Oklahoma","Oregon","Pennsylvania","Rhode Island","South Carolina","South Dakota","Tennessee","Texas","Utah","Vermont","Virginia","Washington","West Virginia","Wisconsin","Wyoming"
)
colnames(Electorial_Votes) <- "Electorial_Votes"
print(Electorial_Votes)
Electorial_Votes <- c(9,3,11,6,55,9,7,3,3,29,16,4,4,20,11,6,6,8,8,4,10,11,16,10,6,10,3,5,6,4,14,5,29,15,3,18,7,7,20,4,9,3,11,38,6,3,13,12,5,10,3)
names(Electorial_Votes) <- c(
  "Alabama","Alaska","Arizona","Arkansas","California","Colorado","Connecticut","Delaware","District of Columbia","Florida","Georgia","Hawaii","Idaho","Illinois","Indiana","Iowa","Kansas","Kentucky","Louisiana","Maine","Maryland","Massachusetts","Michigan","Minnesota","Mississippi","Missouri","Montana","Nebraska","Nevada","New Hampshire","New Jersey","New Mexico","New York","North Carolina","North Dakota","Ohio","Oklahoma","Oregon","Pennsylvania","Rhode Island","South Carolina","South Dakota","Tennessee","Texas","Utah","Vermont","Virginia","Washington","West Virginia","Wisconsin","Wyoming"
)
```

***

## Find the largest number of electorial votes

```yaml
type: NormalExercise
xp: 20
key: 114dfbbdc4
```

`@instructions`
Find the largest number of electorial votes

`@hint`
Type max(Electorial_Votes), then press the submit button

`@solution`
```{r}
max(Electorial_Votes)
```

***

## Find which state/district has the largest number of electorial votes

```yaml
type: NormalExercise
xp: 20
key: c5f93b7c62
```

`@instructions`
Find which state/district has the largest number of electorial votes

`@hint`
Type which.max(Electorial_Votes), then press the submit button

`@solution`
```{r}
which.max(Electorial_Votes)
```

***

## Find the least number of electorial votes of state/districts that have a vote

```yaml
type: NormalExercise
xp: 20
key: 73b738a287
```

`@instructions`
Find the least number of electorial votes

`@hint`
Type min(Electorial_Votes), then press the submit button

`@solution`
```{r}
min(Electorial_Votes)
```

***

## Find which state/district has the least number of electorial votes
## Note: There are multiple states with the minimum number of electorial colleges, the which.min() function will grab the first one

```yaml
type: NormalExercise
xp: 20
key: 3efd594881
```

`@instructions`
Find which state/district has the least number of electorial votes

`@hint`
Type which.min(Electorial_Votes), then press the submit button

`@solution`
```{r}
which.max(Electorial_Votes)
```

---

## Using dotplots/stripcharts to see your data

```yaml
type: BulletExercise
lang: r
xp: 100
key: 47fc948fb1
```

Dotplots are visual representations of data that enable quick insights into the collection of numbers. Dotplots are also called stripcharts.

The `dotplot()` function creates dotplots.

The mean of a dataset is the sum of all the numbers divided by the number of observations.
The median is the middle value, or the average of the middle two values.
The mean and median are ways to describe the center of data using only one number.

The median is better than the mean when the data is very skewed.
The mean is better than the median when there are very few distinct observations.
In most situations, the mean is preferred.

The `mean()` function computes the mean.
The `median()` function computes the median.

`@pre_exercise_code`

```{r}
Electorial_Votes <- c(
  9,3,11,6,55,9,7,3,3,29,16,4,4,20,11,6,6,8,8,4,10,11,16,10,6,10,3,5,6,4,14,5,29,15,3,18,7,7,20,4,9,3,11,38,6,3,13,12,5,10,3
)
names(Electorial_Votes) <- c(
  "Alabama","Alaska","Arizona","Arkansas","California","Colorado","Connecticut","Delaware","District of Columbia","Florida","Georgia","Hawaii","Idaho","Illinois","Indiana","Iowa","Kansas","Kentucky","Louisiana","Maine","Maryland","Massachusetts","Michigan","Minnesota","Mississippi","Missouri","Montana","Nebraska","Nevada","New Hampshire","New Jersey","New Mexico","New York","North Carolina","North Dakota","Ohio","Oklahoma","Oregon","Pennsylvania","Rhode Island","South Carolina","South Dakota","Tennessee","Texas","Utah","Vermont","Virginia","Washington","West Virginia","Wisconsin","Wyoming"
)
dotplot <- function(x){
  stripchart(x,xaxt = "n",method = "stack")
  axis(1,at = x,pos = 0.9)
}
```

***

## Create a dotplot/stripchart for the electorial votes dataset

```yaml
type: NormalExercise
xp: 34
key: 1ae58b7838
```

`@instructions`

Use the `dotplot()` function to create a dotplot of the electorial college votes

`@hint`

Type `dotplot(Electorial_Votes)`, then press the submit button.

`@solution`

```{r}
dotplot(Electorial_Votes)
```

***

## Compute the mean electorial college

```yaml
type: NormalExercise
xp: 33
key: 7977e95ddd
```

`@instructions`

Use the `mean()` function to find the average number of electorial college votes

`@hint`

Type `mean(Electorial_Votes)`, then press the submit button.

`@solution`

```{r}
mean(Electorial_Votes)
```

***

## Compute the median electorial college

```yaml
type: NormalExercise
xp: 33
key: 5ce97d9fe7
```

`@instructions`

Use the `median()` function to find the typical number of electorial college votes

`@hint`

Type `median(Electorial_Votes)`, then press the submit button.

`@solution`

```{r}
median(Electorial_Votes)
```

---

## Use a dotplot to determine skew

```yaml
type: BulletExercise
lang: r
xp: 25
key: 6d4cc518f0
```

Data is called skewwed if to one side there is a lot more variability than on the other side.
Symmetric data has approximately equal variance on the left and on the right.

* Dotplots of skewed right data have a tail going to the right.
* Dotplots of skewed left data have a tail going to the left.
* Symmetric data has approximately the same shape on the left and on the right.

Look at the dotplot and decide if the electorial vote numbers are skew left, skew right or symmetric.

`@pre_exercise_code`

```{r}
Electorial_Votes <- c(
  9,3,11,6,55,9,7,3,3,29,16,4,4,20,11,6,6,8,8,4,10,11,16,10,6,10,3,5,6,4,14,5,29,15,3,18,7,7,20,4,9,3,11,38,6,3,13,12,5,10,3
)
names(Electorial_Votes) <- c(
  "Alabama","Alaska","Arizona","Arkansas","California","Colorado","Connecticut","Delaware","District of Columbia","Florida","Georgia","Hawaii","Idaho","Illinois","Indiana","Iowa","Kansas","Kentucky","Louisiana","Maine","Maryland","Massachusetts","Michigan","Minnesota","Mississippi","Missouri","Montana","Nebraska","Nevada","New Hampshire","New Jersey","New Mexico","New York","North Carolina","North Dakota","Ohio","Oklahoma","Oregon","Pennsylvania","Rhode Island","South Carolina","South Dakota","Tennessee","Texas","Utah","Vermont","Virginia","Washington","West Virginia","Wisconsin","Wyoming"
)
dotplot <- function(x){
  stripchart(x,xaxt = "n",method = "stack")
  axis(1,at = x,pos = 0.9)
}
dotplot(Electorial_Votes)
```

***

```yaml
type: MultipleChoiceExercise
xp: 50
key: 260312ca37
```

## Is the electorial vote data skew left, skew right, symmetric, or none of these?

`@instructions`

Look at the dotplot and decide if the electorial vote numbers are skew left, skew right or symmetric.

`@possible_answers`

 - skew left
 - [skew right]
 - symmetric
 - neither skewed nor symmetric
 
 ***

```yaml
type: MultipleChoiceExercise
xp: 50
```

## Would the mean or the median be a better description of the center of the data?

`@instructions`

Look at the dotplot and decide if the electorial vote numbers center would be better described by the mean or the median.

`@possible_answers`

 - mean
 - median
 
 `@hint`
 
 The data is skew right, so the mean is a poor choice.