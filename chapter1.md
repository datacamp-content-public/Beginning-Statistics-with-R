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

## Insert exercise title here

```yaml
type: BulletExercise 
xp: 100 
key: 8fb45ad353   
```


If you


`@pre_exercise_code`

```{r}
Electorial_Votes <- matrix(c(9,3,11,6,55,9,7,3,3,29,16,4,4,20,11,6,6,8,8,4,10,11,16,10,6,10,3,5,6,4,14,5,29,15,3,18,7,7,20,4,9,3,11,38,6,3,13,12,5,10,3),ncol = 1)
rownames(Electorial_Votes) <- c(
  "Alabama","Alaska","Arizona","Arkansas","California","Colorado","Connecticut","Delaware","District of Columbia","Florida","Georgia","Hawaii","Idaho","Illinois","Indiana","Iowa","Kansas","Kentucky","Louisiana","Maine","Maryland","Massachusetts","Michigan","Minnesota","Mississippi","Missouri","Montana","Nebraska","Nevada","New Hampshire","New Jersey","New Mexico","New York","North Carolina","North Dakota","Ohio","Oklahoma","Oregon","Pennsylvania","Rhode Island","South Carolina","South Dakota","Tennessee","Texas","Utah","Vermont","Virginia","Washington","West Virginia","Wisconsin","Wyoming"
)
colnames(Electorial_Votes) <- "Electorial_Votes"
print(Electorial_Votes)
```


`@sample_code`

```{r}

```

