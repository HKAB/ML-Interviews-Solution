# Probability

### 1. Uniform distribution
p(X = 0.5) = 0

### 2. PDF
PDF can be greater than 1, for example uniform distribution in range (0, 1/2) has PDF = 2 when x in (0, 1/2) and 0 else where. To understand more, the probability can be express as: probability = area under distribution curve = base * height = 1\/2\*2 = 1. The PDF can be very large, but the base is small to keep the probability in a range never surpass 1.

### 3. Multimodal vs Multivariate
(This is the first time I heard about Multimodel distribution)
Multimodal distribution is distribution with multi-mode, mean while Multivariate distribution is involved with multiple variable.

### 4. Independence
Two variable A and B are independent if (P(A^B) = P(A)\*P(B)). Intuitively, B does not affect A.

### 5. Normal distribution
If there is an unknown distribution, it might be combined with a lot of other distribution. By the Central Limit Theorem, it converges to Normal distribution.

### 6. Probabilistic model & Deterministic model
We can turn probabilistic model to deterministic by remove the random part. (for example in linear regression, if we remove the bias term, which is assumed being generated from a normal distribution, it will become deterministic)

### 7.

### 8. t-distribution
t-distribution will be useful when the sample size is small or population deviation is unknown. If the sample size (degree of freedom) is high, it approximate normal distribution.

### 9. Poisson distribution
i) We have lambda = 5/12 (times/month). So P_{k=1}(0, 1) = ((\lambda\*t)^k\*e^{\lambda\*t})/k! with t = 1, \lambda = 5/12.
ii) 1 - p_{k=0}(0, t) (?)

### 10. Probability
Call X is the event the classifier is right, we have P(X = 1) ~ 9/10. So the probability that the classifier will predict correctly all 20 upcoming event is ~ (9/10)^20.

### 11.

### 12. Excerices
Let X be the event that Jason have a boy (out of two children): P(X) = (bb + bg + gb)/(bb + bg + gb + gg) = 3/4 (Kid are distinguishable).
Let Z be the event that Jason have two boys.
P(Z|X) = P(X|Z)\*P(Z)/P(X) = P(Z)/P(X) = 1/3

### 13. Excercise
i)
Let A: Event that X was pick up from store A. P(A) = 0.5
Let B: Event that X was pick up from store B. P(B) = 0.5
Let Z: Event that the chip is defective
P(Z) = P(Z|A)\*P(A) + P(Z|B)\*P(B) = 0.3\*0.5 + 0.7\*0.5 = 0.5
ii)
Let A: Event that two chips was pick up from store A. P(A) = 0.5
Let B: Event that two chips was pick up from store B. P(B) = 0.5
Let X: Event that chip 1 function normaly.
Let Y: Event that chip 2 function normaly.

P(Y|X) = P(Y^X)/P(X = (P(Y^X|A)\*P(A) + P(Y^X|B)\*P(B))/(P(X|A)\*P(A) + P(X|B)\*P(B)) = 0.7\*0.7 + 0.3\*0.3 = 0.58

