# haskell-pbt

Playground to see how the examples of "Property-Based Testing with PropEr, Erlang, and Elixir" by Fred Hebert (or variations inspired by those examples) can be implemented in Haskell using quickcheck. It's also a playground for a number of related libraries and topics:
* https://hackage.haskell.org/package/QuickCheck-2.14.2/docs/Test-QuickCheck-Monadic.html
* https://hackage.haskell.org/package/quickcheck-state-machine
* https://hackage.haskell.org/package/dejafu


References:

1. F. Hebert, [Property-Based Testing with PropEr, Erlang, and Elixir](https://pragprog.com/titles/fhproper/property-based-testing-with-proper-erlang-and-elixir/)
1. J. Hughes, [Testing Monadic Code with QuickCheck](https://www.researchgate.net/publication/2831386_Testing_Monadic_Code_with_QuickCheck)
1. M. Walker, C. Runciman, [Déjà Fu: a concurrency testing library for Haskell](https://dl.acm.org/doi/10.1145/2887747.2804306)


## How to build and run locally

The project uses the [Haskell tool stack](https://docs.haskellstack.org/en/stable/README/).

Assuming `stack` is installed in the system, the project can be build by running
```
stack build
```
To build and also run the tests, run
```
stack test
```
which is equivalent to
```
stack build --test
```
To run the executable,
```
stack exec haskell-pbt-exe
```
For a faster feedback loop,
```
stack test --fast --file-watch
```
To run `ghci` (with a version compatible with the resolver) run
```
stack ghci
```
For more information, refer to the `stack` official docs.
