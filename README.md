<!-- Stopped @ 1:03:13 on https://vimeo.com/113588389 -->

# Functional Programming Design Patterns (Mathematics)
Category theory as an abstract branch of math that can formalize concepts from other branches such as Set, Type, Group, Logic and others.
# Monoids and Monads

#### Generalizations

## Monoids satisfy these 3 RULES
- Closure (normally called REDUCE)
    - *The result of combining two things is ALWAYS another one of the things*
    - The type is "closed" since it only accepts the same type it is passed.
    - Any pairwise op can run on lists
- Associativity
    - *When combining more than two things, which pairwise combination you do first doest NOT matter*
    - Any combination of monoids 
    is also a monoid
    - Provides for "cool" algorithms
        - Divide and Conquer
        - Parrallelization
            - Multicore operations
        - Incremental Accumulation
            - You can compute now and later

- Identity Element
    - *The ZERO element, such that when combined with anything, you get the original thing back* 

    - a "no-op" fn

    - Zero (0)

    - Empty string
      Returns exactly what you pass in.
    
- What about Functions?
    - > Functions with the same type of input and output are indeed monoids
    - These are called *ENDOMORPHISMS*

** SEMIGROUPS are not MONOIDS as they lack an identity element.

** Given a list and a pairwise operation (binary) we can REDUCE! ☃

** Any function containing an endomorphism in it's signature, can be converted into a monoid.
## Monad