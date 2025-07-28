# Week 0: Functions, Variables

Link to Problem Set 0: https://cs50.harvard.edu/python/2022/psets/0/

**Indoor Voice**
```python
def use_indor_voice(text: str):
    return text.lower();

def main():
    text = input("Use your indoor voice!\n")
    print( use_indor_voice(text) );

main()
```

**Playback Speed**
```python
def payback(text: str):
    return "...".join( text.split() );

def main():
    text = input("Say something:\n")
    print( payback(text) )

main()
```

**Making Faces**
```python
def convert(txt: str):
    return txt.replace(":)", "🙂").replace(":(", "🙁")

def main():
    user_input = input("Say something:\n")
    print(convert(user_input))

main()
```

**Einstein**
```python
def calulate(m):
    return int(m) * 300000000 ** 2

def main()
    m = input("Insert m value: ")
    print(f"E = { caluclate(m) }")
```

**Tip Calculator**
```python
def main():
    dollars = dollars_to_float(input("How much was the meal? "))
    percent = percent_to_float(input("What percentage would you like to tip? "))
    tip = dollars * percent
    print(f"Leave ${tip:.2f}")

def dollars_to_float(d):
    return float(d.replace("$", ""))

def percent_to_float(p):
    return float(p.replace("%",""))/100

main()
```
