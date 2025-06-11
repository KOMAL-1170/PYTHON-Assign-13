# Dictionary of students and their marks in 5 subjects
students = {
    "Alice": [85, 78, 92, 88, 76],
    "Bob": [72, 68, 75, 70, 69],
    "Charlie": [90, 95, 93, 89, 94],
    "Diana": [60, 65, 58, 62, 64],
    "Ethan": [80, 82, 85, 79, 83]
}

# Dictionary to store averages
averages = {}

# Calculate average for each student
for name, marks in students.items():
    avg = sum(marks) / len(marks)
    averages[name] = avg

# Find student with max and min average
max_student = max(averages, key=averages.get)
min_student = min(averages, key=averages.get)

print(f"Student with Maximum Average: {max_student} ({averages[max_student]:.2f})")
print(f"Student with Minimum Average: {min_student} ({averages[min_student]:.2f})")
