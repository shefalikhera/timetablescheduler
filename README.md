# Timetable Scheduler

## Overview
Timetable Scheduler is a Java-based application designed to create and manage class schedules for an educational institution. It allows users to input subjects, allocate class types (lecture, lab, or tutorial), and edit schedules with flexibility, ensuring no conflicts in allocated slots.

---

## Features
1. **Subject Input:**
   - Users can input the number of subjects and their names.

2. **Class Scheduling:**
   - Allocate classes as lectures, labs, or tutorials based on user input.
   - Ensures no conflict between scheduled classes and prevents overlapping.

3. **Conflict Management:**
   - Verifies if a lab or tutorial is already scheduled for a subject.
   - Avoids scheduling conflicts by checking slot availability.

4. **Timetable Editing:**
   - Allows users to edit the schedule by specifying the day and slot.
   - Prevents edits that disrupt ongoing labs or tutorials.

5. **Timetable Display:**
   - Prints the timetable in a well-organized format, showing scheduled classes or free slots.

---

## Installation
1. **Requirements:**
   - Java Development Kit (JDK) 8 or above.
   - Integrated Development Environment (IDE) like IntelliJ IDEA, Eclipse, or VS Code.

2. **Setup:**
   - Copy the provided source code into your IDE.
   - Compile and run the program.

---

## Code Structure
- **Main Class:**
  - `TimetableScheduler`: Entry point of the application. Handles user input and invokes scheduling and editing methods.

- **Methods:**
  - `scheduleClasses`: Allocates slots for lectures, labs, or tutorials based on subject and user choice.
  - `checkLaborTut`: Checks if a lab or tutorial is already scheduled for a subject.
  - `editTimetable`: Allows editing of scheduled slots while maintaining consistency.
  - `isEditAllowed`: Ensures edits don’t disrupt ongoing multi-slot classes like labs or tutorials.
  - `isClassScheduled`: Checks if a class is already scheduled for a subject on a specific day.
  - `isSlotAvailable`: Verifies slot availability for the required number of continuous slots.
  - `printTimetable`: Prints the timetable in a user-friendly format.

---

## Usage
1. **Run the Program:**
   - Execute the `TimetableScheduler` class.

2. **Input Subjects:**
   - Specify the number of subjects and their names.

3. **Schedule Classes:**
   - Choose the class type for each subject and allocate slots.

4. **Edit Timetable:**
   - Modify the timetable by specifying the day and slot.

5. **View Timetable:**
   - Display the timetable to review the schedule.

---

## Sample Output
### Initial Input
```
Enter the number of subjects: 3
Enter subject 1: Math
Enter subject 2: Physics
Enter subject 3: Chemistry
```

### Timetable Display
```
Mon: Math           Free           Free           Physics        Free           Free           Free
Tue: Free           Free           Free           Chemistry      Free           Free           Free
Wed: Math           Math           Math           Free           Free           Free           Free
Thu: Free           Free           Free           Free           Free           Free           Free
Fri: Free           Free           Free           Free           Free           Free           Free
```

### Edit Example
```
Enter day and slot to edit (e.g., Mon 3), or 'exit' to finish: Tue 4
Enter the new subject or 'free' to clear the slot: Free
Updated Timetable:
Tue: Free           Free           Free           Free           Free           Free           Free
```

---

## Contributors
- **Shefali Khera**

---

## Notes
1. Ensure valid input for day names and slot numbers.
2. Lab and tutorial slots require continuous free slots.
3. Editing between multi-slot classes is restricted to maintain consistency.

---


