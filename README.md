The outputs (as "output.txt")
from previous iterations of the tests for each context-free
language are under folders `1`-`11` under `cfg_tests`. The articulation
attempts can also be found there.

### Setup
Have a python environment in which the `openai` package is installed, via
`pip install openai`. Have an OpenAI API key with access to GPT-4. Copy this
API key
to a file called `key.txt` in this folder.

### Running classification Tests
With setup done, run `python gen_classification.py [pattern number you want to test]`
from this folder.

### Running articulation Attempts
With setup done, run `python gen_articulation.py [pattern number you want to test]`
from this folder.

### Running faithfulness testing by chain-of-reasoning injection
To bring up the interface where, for a given pattern, you will be able to run
classification on random test strings both with and without chain-of-reasoning
injection, run `python faithfulness_test.py [pattern number]`. Follow the
instructions on the prompt. Note that backspace will not display properly
on Python `input()` prompts.
