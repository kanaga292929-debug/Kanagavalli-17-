# A simple implementation of a Stack using a List
class Stack:
    def __init__(self):
        self.items = []

    def push(self, item):
        """Adds an element to the top of the stack."""
        self.items.append(item)
        print(f"Pushed: {item}")

    def pop(self):
        """Removes the top element from the stack."""
        if not self.is_empty():
            return self.items.pop()
        return "Stack is empty!"

    def is_empty(self):
        return len(self.items) == 0

# Demo
my_stack = Stack()
my_stack.push(10)
my_stack.push(20)
print(f"Popped: {my_stack.pop()}")
# Kanagavalli-17-
