# **Dunder (Magic, Special) Methods**

- Dunder methods are special methods that are prefixed with double underscores.
- Dunder methods are used to provide a way to access the internal state of an object.

- Dunder methods let you emulate the behavior of built-in types. For example, to get the length of a string you can call len('string'). But an empty class definition doesn’t support this behavior out of the box:

```
        class LenSupport:
            def __len__(self):
                return 42

        >>> obj = LenSupport()
        >>> len(obj)
        42
```

![](https://miro.medium.com/max/1838/1*g6LbGqMogPuFiHojMmSFTw.png)


### Context Manager Support and the With Statement: __enter__, __exit__:

-A context manager is a simple “protocol” (or interface) that your object needs to follow so it can be used with the with statement. Basically all you need to do is add __enter__ and __exit__ methods to an object if you want it to function as a context manager.

```
    class Account:
        # ... (see above)

        def __enter__(self):
            print('ENTER WITH: Making backup of transactions for rollback')
            self._copy_transactions = list(self._transactions)
            return self

        def __exit__(self, exc_type, exc_val, exc_tb):
            print('EXIT WITH:', end=' ')
            if exc_type:
                self._transactions = self._copy_transactions
                print('Rolling back to previous transactions')
                print('Transaction resulted in {} ({})'.format(
                    exc_type.__name__, exc_val))
            else:
                print('Transaction OK')
```

## **Basic Statistics in Python — Probability**:

What is probability?
- In simple words probability answers the question of “What is the chance of an event happening?”
-  To calculate the chance of an event happening, we also need to consider all the other events that can occur. The quintessential representation of probability is the humble coin toss. 

- In a coin:
1. Flipping a heads
2. Flipping a tails 

- By looking at the events that can occur, probability gives us a framework for making predictions about how often events will happen.

- This example shows how probabilities of flipping heads:
```
    import random
    def coin_trial():
    heads = 0
    for i in range(100):
        if random.random() <= 0.5:
            heads +=1
        return heads
    def simulate(n):
        trials = []
        for i in range(n):
            trials.append(coin_trial())
        return(sum(trials)/n)
    simulate(10)
    >>> 5.4
    simulate(100)
    >>> 4.83
    simulate(1000)
    >>> 5.055
    simulate(1000000)
    >>> 4.999781
```



# The data and the distribution:

- The normal distribution refers to a particularly important phenomenon in the realm of probability and statistics.

- The most important qualities to notice about the normal distribution is its symmetry and its shape. We’ve been calling it a distribution, but what exactly is being distributed? It depends on the context. In probability, the normal distribution is a particular distribution of the probability across all of the events. The x-axis takes on the values of events we want to know the probability of. The y-axis is the probability associated with each event, from 0 to 1.

- The normal distribution is significant to probability and statistics thanks to two factors: the Central Limit Theorem and the Three Sigma Rule.

    ![](https://i.imgur.com/egqrj58.jpg)

- In a probability context, the high point in a normal distribution represents the event with the highest probability of occurring.

## **Three Sigma Rule**

- The Three Sigma rule, also known as the empirical rule or 68-95-99.7 rule, is an expression of how many of our observations fall within a certain distance of the mean. Remember that the standard deviation (a.k.a. “sigma”) is the average distance an observation in the data set is from the mean

![](https://pbs.twimg.com/media/Dg3-YbjVAAA69YX.jpg)

## **Z-score**

- The Z-score is a simple calculation that answers the question, “Given a data point, how many standard deviations is it away from the mean?
- The equation below is the Z-score equation.

![](https://www.simplypsychology.org/Z-score-formula.jpg?ezimgfmt=rs:382x312/rscb26/ng:webp/ngcb26)