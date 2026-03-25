# Student Grade Calculator

print("Student Grade Calculator")

# Input marks
tamil = 80
english = 75
maths = 90
science = 85
social = 70

# Calculate total and average
total = tamil + english + maths + science + social
average = total / 5

print("Total Marks:", total)
print("Average:", average)

# Find grade
if average >= 90:
    print("Grade: A")
elif average >= 75:
    print("Grade: B")
elif average >= 60:
    print("Grade: C")
else:
    print("Grade: D")
