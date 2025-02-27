# Dictionary Best Practice

## Mistake #1: Wrong way to check if a key exists

Sometimes people do this to check if the key exists or not:

```python
my_dict = {"name": "Kiran", "age": 24}
if "name" in my_dict:
    print(my_dict["name"])
else:
    print("No name found")
```

A better way to do this:

```python
my_dict = {"name": "Kiran", "age": 24}
print(my_dict.get("name", "No name found"))
```

This method makes the code cleaner by removing the extra if-else checks.

## Mistake #2: Incorrect looping over both keys and values

Many people loop like this:

```python
my_dict = {"a": 1, "b": 2, "c": 3}
for key in my_dict:
    print(key, my_dict[key])  
```

A better approach:

```python
for key, value in my_dict.items():
    print(key, value)
```

This makes the code more readable and efficient.

## Mistake #3: Incorrect way of merging dictionaries

Some beginners merge dictionaries like this:

```python
dict1 = {"a": 1, "b": 2}
dict2 = {"b": 3, "c": 4}
dict1.update(dict2)
print(dict1)
```

This modifies `dict1` in place. Instead, use dictionary unpacking:

```python
dict1 = {"a": 1, "b": 2}
dict2 = {"b": 3, "c": 4}
new_dict = {**dict1, **dict2}
print(new_dict)  # {'a': 1, 'b': 3, 'c': 4}
```

This creates a new dictionary, avoiding accidental modifications.

## Mistake #4: Overusing `defaultdict`

Example of unnecessary `defaultdict` usage:

```python
from collections import defaultdict
my_dict = defaultdict(int)
my_dict["a"] += 1  # Works, but is it needed?
```

A simpler approach:

```python
my_dict = {}
my_dict["a"] = my_dict.get("a", 0) + 1
```

This avoids unnecessary imports and keeps the code simple.

## Mistake #5: Ignoring dictionary performance

When dealing with large dictionaries:

```python
my_dict = {i: i**2 for i in range(10_000_000)}  
```

This consumes a lot of memory. Instead, use a generator:

```python
def squared_numbers():
    for i in range(10_000_000):
        yield i, i**2

my_dict = dict(squared_numbers())
```

This approach reduces memory usage.

## Mistake #6: Misusing `setdefault()`

Beginners often do this:

```python
data = {}
if "name" not in data:
    data["name"] = "kiran"
```

A better way:

```python
data = {}
data.setdefault("name", "kiran")
```

However, using `setdefault()` incorrectly can waste time:

```python
name = data.setdefault("name", some_expensive_function())
```

Even if "name" is present, `some_expensive_function()` is still executed. Instead, use:

```python
name = data.get("name", "kiran")
```

## Mistake #7: Not using `Counter` for counting

Many beginners count items manually:

```python
words = ["apple", "banana", "apple"]
word_count = {}
for word in words:
    word_count[word] = word_count.get(word, 0) + 1
```

A better approach using `Counter`:

```python
from collections import Counter
word_count = Counter(words)
```

This makes the code cleaner and more efficient.

---

By following these best practices, your Python dictionary usage will become more efficient and readable!

