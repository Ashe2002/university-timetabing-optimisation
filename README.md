# University_Timetabling
This repository contains a report detailing an attempt to carry out the timetabling for the University of Edinburgh. The goal is to schedule all "events" (Lectures, Workshops, Tutorials, etc..) to a timeslot and room, such that resource constraints are satisfied and soft constraint violations are minimised. 

We explored scheduling the timetabling in the standard case (Monday-Friday, 9-6) in addition to the cases where we (1) remove friday afternoon teaching, (2) remove teaching from 5-6, (3) remove both. We also experimented with both 30 minute and 60 minute timeslots for events. Due to the scale of the challenge two approaches were taken, an exact Mixed Integer Programming approach, and a heuristic approach. In the MIP case, we split the university into smaller campuses and completed schedules for the Kings Buildings (KB), Easter Bush (EB) and BioQuarter (BQ) campuses.

The three CSV files hold the cleaned data used for the timetabling. Then there is a ipynb file for each (campus, semester, timeslot, day-length) combination. These files generate CSVs for the results of the timetabling.
