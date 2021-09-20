# (Same-Message Linkable) Extendable (Threshold) Ring Signatures

This repository contains a fork of the RELIC library implementing extendable (threshold) ring signatures.
It is meant to be a research prototype for reproducibility, and not for production purposes.

The repository contains:
- An implementation of the schemes in files `relic/src/cp/relic_cp_ers.c` (for the extendable), `relic/src/cp/relic_cp_smlers.c` (for the same-message-linkable) and `relic/src/cp/relic_cp_etrs.c` (for the threshold version)
- Basic tests and benchmarks in the `relic/test/test_cp.c` and `relic/bench/bench_cp.c` programs
- A demo program to print performance figures from the implementation as JSON files

## Build Instructions

The easiest way to reproduce results is running `make` inside the `relic/demo/ers-etrs` folder.

This will build a self-contained version of RELIC and link a testing/benchmarking program against the library.

## Benchmarking

Running `relic/demo/ers-etrs/test-bench` will print a series of JSON files with the performance figures used in the paper.

## LICENSE

This code is released under the Apache 2.0 License.
