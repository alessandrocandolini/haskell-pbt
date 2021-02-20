# haskell-pbt

Playground to see how the examples of "Property-Based Testing with PropEr, Erlang, and Elixir" by Fred Hebert can be implemented in Haskell using quickcheck. It's also a playground for a number of related libraries and topics:
* quickcheck monadicIO 
* https://hackage.haskell.org/package/quickcheck-state-machine
* https://hackage.haskell.org/package/dejafu


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
