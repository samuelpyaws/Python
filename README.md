# Python
#Access specifiers
#class Person:
    def __init__(self):
        self.name = "samuel"      # Public
        self._age = 25          # Protected
        self.__salary = 50000   # Private

    def display(self):
        print(self.name)
        print(self._age)
        print(self.__salary)

p = Person()

print(p.name)        # Public
print(p._age)        # Protected (accessible)
#print(p.__salary)  # Error

print(p._Person__salary)  # Private accessed via name mangling
