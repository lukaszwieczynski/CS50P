# HarvardX CS50P's Introduction to Programming with Python

### Week 1: Conditionals

Link to Problem Set 1: https://cs50.harvard.edu/python/2022/psets/1/

**Deep Thought**
```python
def main():
    text = input("What is the Answer to the Great Question of Life, the Universe, and Everything? ")

    try:
        answer = int(text) == 42
    except ValueError:
        answer = (text == "forty two" or text == "forty-two")
    
    print("Yes" if answer else "No")

main()
```

**Home Federal Savings Bank**
```python
def main():
    greeting = input("Greeting: ");

    if greeting.startswith("Hello"):
        print("$0");
    elif greeting.startswith("H"):
        print("$20");
    else:
        print("$100")
main()
```

**File Extensions**
```python
import mimetypes

def main():
    file_name = input("Please enter the file name with extension: ");
    file_extension = file_name.split('.')[-1] if '.' in file_name else '';
    print(mimetypes.types_map.get(f".{file_extension}", 'Unknown MIME type'));

main()
```

**Math Interpreter**
```python
def main():
    x, y, z = input("Please enter the file name with extension: ").split(" ");

    if y == "+":
        print("{:.2f}".format(int(x) + int(z)))
    elif y == "-":
        print("{:.2f}".format(int(x) - int(z)))
    elif y == "*":
        print("{:.2f}".format(int(x) * int(z)))
    elif y == "/":
        if int(z) == 0:
            print("Cannot divide by zero.")
        else:
            print("{:.2f}".forat(int(x) / int(z)))
    else:
        print("Unknown operation.")
main()
```

**Meal Time**
```python
def main():
    time = input("What time is it? ");
    time = convert(time);

    if time <= 8 and time >= 7:
        print("breakfast time");
    elif time <= 13 and time >= 12:
        print("lunch time");
    elif time <= 19 and time >= 18:
        print("dinner time");

def convert(time: str):
    hh, mm = time.split(":");
    return float(int(hh) + int(mm) / 60);

main()
```
