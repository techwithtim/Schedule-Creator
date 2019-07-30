# Schedule-Creator
A schedule creator used to create timetables for a summer camp. Created using python and the Qt Library.

# Running The Program
To run the program simply execute the script *ui.py*.

# Program Information
**Purpose** 
This scheduling software was used by the office
staff at one of my previous jobs, a summer camp. It was
used to generate a set of group schedules for campers based
on a variety of constraints given to me.
 
**Schedule Layout**
The schedule for each group has 6 periods.
2 in the morning and 4 in the afternoon. The morning contains 2 sports.
While the afternoon consists of a lunch, a swim and 2 sports. Lunch and swim
will always happen the same period each day.

**Schedule Rules**
Each schedule has a set of rules that must be followed if possible.
- No group may have the same activity more than 3 times a week (2 if possible)
- No group may have the same activity on the same day
- No two groups can have the same activty at the same time 
- If an activity exists twice in a week it should be at least one day apart from
  the last time it occured 
- If an activty exists more than twice in a week it should be in the oppsoite part
    of the day. Meaning if for example: soccer occurs in the monring, then if it occurs
    again it will be in the afternoon
- Group 2 will never place tennis

**Details**
Each week the office staff manually create a schedule 
for each group of campers expected in the following week. The goal
when creating this schedule is to keep each one as diverse as possible.
Meaning that each group particiaptes in as many activites as possible. This
is tedious and very difficult to do. Having sometimes up to 10 groups a week
doing this effectively becomes very diffuclt due to the mathematical complexity
of balancing activities between the groups and within the individual schedules.
I compare it to solving a more advanced version of sudoku.

**Limitations** 
Sometimes the constraints selected in the program
interface are impossible to generate a schedule for. Take for example
the case in which you have 10 groups and only 8 activities available in
the morning. Since no activity can run at the same time the schdule is
impossible to generate.
