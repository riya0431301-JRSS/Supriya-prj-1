from student import Student
from database import Database

db = Database()

def menu():
    while True:
        print("\n1. Add Student")
        print("2. View Students")
        print("3. Exit")

        choice = input("Enter choice: ")

        if choice == '1':
            name = input("Enter name: ")
            age = input("Enter age: ")
            student = Student(name, age)
            db.add_student(student)

        elif choice == '2':
            students = db.get_students()
            for s in students:
                print(f"Name: {s.name}, Age: {s.age}")

        elif choice == '3':
            break

menu()
