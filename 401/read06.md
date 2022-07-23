# Ten Thousand Game 1

## Random Module

Information from [pythonforbeginner.com](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)

The random module in Python allows a developer to generate random numbers. This module is useful in many ways including: video games, websites, and applications. Random comes with many functions such as:

- Randint -> finds a random integer in between a given range of numbers
- Random -> Finds a large random integer by multiplying the function by a number ex: `random.random() * 100`
- Shuffle -> Shuffles the elements of a list in place so they are in a random order
- Randrange -> Generates a randomly selected element from a range (start, stop, step)

---

## Risk Analysis

Information from [edureka.co](https://www.edureka.co/blog/risk-analysis-in-software-testing/)

Risk is defined as the probability of unwanted incidents in a software package. Risk analysis is observing your code and identifying potential unwanted incidents and building your tests based on those incidents.

Causes of new risks to encounter:

1. New hardware
2. New technology
3. New automation tool
4. Sequence of code
5. Test resources

Unavoidable risks:

1. Time allocated for testing
2. Defect leakage due to the complexity or size of the application
3. Urgency from the clients to deliver the project
4. Incomplete requirements

Types of risk:

1. Business Risk
2. Testing Risks
3. Premature Release Risk
4. Software Risks

---

## Test Coverage

Information from [martinfowler.com](https://martinfowler.com/bliki/TestCoverage.html)

When creating code it is important to analyze how much of the code is acually being covered by tests. The question arrizes when testing code: do you have 90% coverage with quality tests or 100% coverage with simple tests? which is better. Martin Fowler (author) suggests the best way to tell if your tests are sufficient is if:

1. You rarely get bugs that escape into production
2. You are rarely hesitant to change some code for fear it will cause production bugs.

---

## Big O Notation

In the video by HackerRank, called "Big O Notation" the speaker goes over the four steps to determining Big O notation.

1. Different steps get added
2. Drop constants
3. Different inputs => different variables
4. Drop non-dominant terms

---

## Python Random

This information is from the [python](https://docs.python.org/3.10/library/random.html) documentation. The documents contain a wealth of functions that the random module offers a list is below:

- random.seed(a=None, version=2)
- random.getstate()
- random.setstate(state)
- random.randbytes(n)
- random.randrange(stop)
- random.randrange(start, stop[, step])
- random.randint(a, b)
- random.getrandbits(k)
- random.choice(seq)
- random.choices(population, weights=None, *, cum_weights=None, k=1)
- random.shuffle(x[, random])
- random.sample(population, k, *, counts=None)
- random.random()
- random.uniform(a, b)
- random.triangular(low, high, mode)
- random.betavariate(alpha, beta)
- random.expovariate(lambd)
- random.gammavariate(alpha, beta)
- random.gauss(mu, sigma)
- random.lognormvariate(mu, sigma)
- random.normalvariate(mu, sigma)
- random.vonmisesvariate(mu, kappa)
- random.paretovariate(alpha)
- random.weibullvariate(alpha, beta)
- class random.Random([seed])
- class random.SystemRandom([seed])

## Things I want to learn more about

Out of all of the articles. What I am most curious about is the Test Coverage article because he slightly contradicts the Test Driven Development(TDD) method saying that if that it will result in poor testing and/or poor code.
