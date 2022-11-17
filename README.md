# my-spring-boot-domo
This repository contains experimentation with combinations of random projection, translation, and additive noiseas a method for performing privacy-preserving data stream mining (tested against known input-output attacks) inan online learning context.


if you have Docker installed, you can run the experiments contained within this codebase by executing makejupyter , opening the returned URL in a web browser, and executing the contents of the provided Jupyternotebooks (This has only been tested on an Ubuntu 16.04 host running Docker 17.05.0-ce).
You wil need to run the notebooks in the "dataset-construction" sub-folder before the notebooks that depend onthose datasets. Note that the results of each experiment are saved to disk to prevent the need to re-execute theexperiments when re-viewing an experiment's results.

**Running Tests**

make run-tests
Tests can also be run repeatedly from a Clojure REPL:

1. lein repl

2.(use 'midje.repl)
