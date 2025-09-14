# AirBnB Clone

This project represents the initial phase in developing a basic replica of the AirBnB platform. The focus here is on constructing a command-line interface (a terminal application) using Python. This interface enables users to create, modify, remove, and handle objects that symbolize various components of the AirBnB ecosystem (such as users, locations, regions, etc.). All information is stored in a JSON file to ensure data persistence.

The primary objectives of this project include:

* Mastering object-oriented programming concepts in Python.
* Managing data serialization and deserialization processes (transforming objects to and from JSON format).
* Developing a fundamental storage system.
* Gaining experience with command-line interface implementation.

---

## The Command Interpreter

The console functions as a compact shell environment. It enables you to engage with the models using straightforward commands.

### Get Started

1. Clone repository and navigate to root directory:

```bash
git clone <https://github.com/Niyigena-Yves/alu-AirBnB_clone.git>

cd alu-AirBnB_clone
```

2. Run the console:

```bash
python3 console.py
```

3. You should see the prompt:

```
(hbnb)
```

Now you can start typing commands!

---

### How to Use It

Here are some of the main commands:

* `create <ClassName>` → creates a new object and prints its id.
* `show <ClassName> <id>` → shows the details of an object.
* `destroy <ClassName> <id>` → deletes an object.
* `all [ClassName]` → shows all objects (or all of a class).
* `update <ClassName> <id> <attr_name> "<attr_value>"` → updates an attribute of an object.
* `quit` or `EOF` → exits the console.

---

### Examples

```
(hbnb) create BaseModel
1234-5678-9012

(hbnb) show BaseModel 1234-5678-9012
[BaseModel] (1234-5678-9012) {'id': '1234-5678-9012', 'created_at': '2025-09-14T03:00:00', 'updated_at': '2025-09-14T03:00:00'}

(hbnb) update BaseModel 1234-5678-9012 name "yves"
(hbnb) show BaseModel 1234-5678-9012
[BaseModel] (1234-5678-9012) {'id': '1234-5678-9012', 'created_at': '2025-09-14T03:00:00', 'updated_at': '2025-09-14T03:07:00', 'name': 'yves'}

(hbnb) all BaseModel
["[BaseModel] (1234-5678-9012) {...}"]

(hbnb) quit
```

---


