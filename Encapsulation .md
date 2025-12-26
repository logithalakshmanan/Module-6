# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
class student:
    def __init__(self, name, age):
        self.name = name
        self.age = age
        self.__rollno = None   # private variable

    def set_rollno(self, r):
        if r > 0:
            self.__rollno = r
        else:
            print("Invalid roll no. Please set correct roll number")

    def get_rollno(self):
        return self.__rollno

    def show(self):
        print("Student Details:", self.name, self.age)

s = student("Jessa", 10)
s.show()

s.set_rollno(-5)   # invalid
s.age = 25
s.show()


## Output
Expected	Got	
Student Details: Jessa 10
Invalid roll no. Please set correct roll number
Student Details: Jessa 25
Student Details: Jessa 10
Invalid roll no. Please set correct roll number
Student Details: Jessa 25

## Result
To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth` is verified
