# HarvardX CS50P's Introduction to Programming with Python

### Week 2: Loops

Link to Problem Set 2: https://cs50.harvard.edu/python/2022/psets/2/

**camelCase**
```python
def main():
    snake_case = ""
    camel_case = input("camelCase: ")

    for char in camel_case:
        if char.isupper():
            snake_case += "_" + char.lower()
        else:
            snake_case += char

    print(snake_case)

main()
```

**Coke Machine**
```python
def main():
    amount_due = 50
    inserted_coins = 0

    while inserted_coins < 50:
        print(f"Amount Due: {amount_due}")

        coin = int(input("Insert Coin: "))

        if coin in [5, 10, 25]:
            inserted_coins += coin
            amount_due -= coin

    change = inserted_coins - 50
    print(f"Change Owed: {change}")
main()
```

**Just setting up my twttr**
```python
def main():
    input_text = input("Input: ")
    output_text = ""

    for char in input_text:
        if char.lower() in ['a', 'e', 'i', 'o', 'u']:
            continue
        else:
            output_text += char

    print(f"Output: {output_text}")
main()
```

**Vanity Plates**
```python
def main():
    plate = input("Plate: ")
    if is_valid(plate):
        print("Valid")
    else:
        print("Invalid")

def is_valid(s):
    if len(s) < 2 or len(s) > 6:
        return False
    if not s[0].isalpha() or not s[1].isalpha():
        return False
    for char in s[2:]:
        if not char.isalnum():
            return False
    return True

main()
```

**Nutrition Facts**
```python
nutrition_facts = {
    "apple": 130,
    "avocado": 50,
    "banana": 110,
    "cantaloupe": 50,
    "grapefruit": 60,
    "grapes": 90,
    "honeydew melon": 50,
    "kiwifruit": 90,
    "lemon": 15,
    "lime": 20,
    "nectarine": 60,
    "orange": 80,
    "peach": 60,
    "pear": 100,
    "pineapple": 50,
    "plums": 70,
    "strawberries": 50,
    "sweet cherries": 100,
    "tangerine": 50,
    "watermelon": 80
}

def main():
    fruit = input("Enter a fruit: ").lower()
    if fruit in nutrition_facts:
        calories = nutrition_facts[fruit]
        print(f"Calories: {calories}")

main()
```
