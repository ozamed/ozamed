<h3>
    
```python
​
import json
from dataclasses import asdict, dataclass


@dataclass
class Stack:
    languages   : tuple = ("Python", "C#","C","C++","SCL")
    databases   : tuple = ("PostgreSQL", "MongoDB", "SQLite")
    workingon   : tuple = ("Machine Learning", "Neural Networks", "Data Science")

    def serialize(self):
        return json.dumps(asdict(self), indent=4)


stack = Stack()
print(stack.serialize())


```
</h3>
