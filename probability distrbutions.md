### 1. Binomial Distribution
- **PMF (Probability Mass Function)**:
  \[
  P(X = k) = \binom{n}{k} p^k (1 - p)^{n - k}
  \]
  where \( n \) is the number of trials, \( k \) is the number of successes, and \( p \) is the probability of success in a single trial.

- **Mean**:
  \[
  \mu = n \cdot p
  \]

- **Standard Deviation**:
  \[
  \sigma = \sqrt{n \cdot p \cdot (1 - p)}
  \]

---

### 2. Hypergeometric Distribution
- **PMF**:
  \[
  P(X = k) = \frac{\binom{K}{k} \binom{N - K}{n - k}}{\binom{N}{n}}
  \]
  where \( N \) is the population size, \( K \) is the number of successes in the population, \( n \) is the number of draws, and \( k \) is the number of successes in the sample.

- **Mean**:
  \[
  \mu = \frac{nK}{N}
  \]

- **Standard Deviation**:
  \[
  \sigma = \sqrt{n \cdot \frac{K}{N} \cdot \frac{N - K}{N} \cdot \frac{N - n}{N - 1}}
  \]

---

### 3. Multinomial Distribution
- **PMF**:
  \[
  P(X_1 = x_1, X_2 = x_2, \dots, X_k = x_k) = \frac{n!}{x_1! x_2! \dots x_k!} p_1^{x_1} p_2^{x_2} \dots p_k^{x_k}
  \]
  where \( n \) is the number of trials, \( x_i \) is the number of successes for category \( i \), and \( p_i \) is the probability of category \( i \).

- **Mean** (for each category \( i \)):
  \[
  \mu_i = n \cdot p_i
  \]

- **Standard Deviation** (for each category \( i \)):
  \[
  \sigma_i = \sqrt{n \cdot p_i \cdot (1 - p_i)}
  \]

---

### 4. Negative Binomial Distribution
- **PMF**:
  \[
  P(X = k) = \binom{k + r - 1}{k} p^r (1 - p)^k
  \]
  where \( r \) is the number of successes, \( k \) is the number of failures, and \( p \) is the probability of success.

- **Mean**:
  \[
  \mu = \frac{r(1 - p)}{p}
  \]

- **Standard Deviation**:
  \[
  \sigma = \sqrt{\frac{r(1 - p)}{p^2}}
  \]

---

### 5. Geometric Distribution
- **PMF**:
  \[
  P(X = k) = (1 - p)^{k - 1} p
  \]
  where \( k \) is the number of trials until the first success, and \( p \) is the probability of success.

- **Mean**:
  \[
  \mu = \frac{1}{p}
  \]

- **Standard Deviation**:
  \[
  \sigma = \frac{\sqrt{1 - p}}{p}
  \]

---

### 6. Poisson Distribution
- **PMF**:
  \[
  P(X = k) = \frac{\lambda^k e^{-\lambda}}{k!}
  \]
  where \( \lambda \) is the average number of occurrences in a fixed interval, and \( k \) is the actual number of occurrences.

- **Mean**:
  \[
  \mu = \lambda
  \]

- **Standard Deviation**:
  \[
  \sigma = \sqrt{\lambda}
  \]

---

### 7. Uniform Distribution (Discrete)
- **PMF**:
  \[
  P(X = x) = \frac{1}{b - a + 1}
  \]
  where \( a \leq x \leq b \) are the possible outcomes in the range.

- **Mean**:
  \[
  \mu = \frac{a + b}{2}
  \]

- **Standard Deviation**:
  \[
  \sigma = \sqrt{\frac{(b - a + 1)^2 - 1}{12}}
  \]

---

### 8. Bayes' Theorem (Posterior Distribution)
- **Bayes' Theorem**:
  \[
  P(H \mid E) = \frac{P(E \mid H) P(H)}{P(E)}
  \]
  where \( P(H \mid E) \) is the posterior probability of hypothesis \( H \) given evidence \( E \), \( P(E \mid H) \) is the likelihood, \( P(H) \) is the prior probability, and \( P(E) \) is the marginal likelihood.

- **Mean and Standard Deviation**: These depend on the form of the posterior distribution after applying Bayes’ theorem. For example, for a normal posterior distribution, the mean and standard deviation are its parameters.
