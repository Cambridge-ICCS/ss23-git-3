# Python RPN calculator

Usage:

```
python rpn_calc.py
```

It will read from `stdin` breaking the input into space-separated tokens.  The
tokens are currently `"+", "-", "*", "/", "p"`.  The "p" token will pop the top
of the stack and print it.  Any other token will be parsed as a floating point
number.  At input end, the top of the stack will be popped and printed.

## Installation (including `pytest` for testing)
```
git clone https://github.com/Cambridge-ICCS/ss23-git-2.git
cd ss23-git
python -m venv venv
source venv/bin/activate
pip install pytest
cd rpn_calc/src
```

## Example
```
python rpn_calc.py << EOM
1 2 +
EOM
3.0
```
