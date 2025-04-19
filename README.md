### Python List Operations Guide
A quick reference for working with lists in Python, including nested lists.

## 📌 Table of Contents
Basic List Operations

Inserting into Nested Lists

Common Pitfalls

## How to Run

# ✨ Basic List Operations
1. Inserting Elements
python
my_list = [10, 20, 30, 40]
my_list.insert(1, 15)  # Insert 15 at index 1
print(my_list)         # Output: [10, 15, 20, 30, 40]
3. Adding Multiple Values
python
my_list.extend([50, 60])  # Add multiple values
print(my_list)            # Output: [10, 15, 20, 30, 40, 50, 60]
🌀 Inserting into Nested Lists
Example: Insert into Inner List
python
nested_list = [[10, 20, 30], [40, 50]]
nested_list[0].insert(1, 15)  # Insert 15 into the first inner list
print(nested_list)            # Output: [[10, 15, 20, 30], [40, 50]]
⚠️ What NOT to Do
python
nested_list = [[10, 20, 30]]
nested_list.insert(1, 15)     # ❌ Adds 15 to the OUTER list
print(nested_list)            # Output: [[10, 20, 30], 15] (Not what you wanted!)
🚨 Common Pitfalls
insert() returns None

python
new_list = my_list.insert(1, 99)  # ❌ new_list = None
Use insert() on its own line; it modifies the list in-place.

extend() vs append()

extend([...]) adds multiple items.

append(x) adds a single item (even if it's a list).

⚡ How to Run
Save the code to a file (e.g., list_operations.py).

Run in terminal:

bash
python list_operations.py
📜 License
MIT © [CharlesMuthui]

🔗 Further Reading
Python Lists (Official Docs)

Mastering Nested Lists

🎉 Happy Coding!


