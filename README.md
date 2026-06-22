# University Timetabling Optimisation

Exact and heuristic approaches to scheduling University of Edinburgh teaching
events across timeslots and rooms.

## Overview

This group project investigates a large university timetabling problem. Lectures,
tutorials, workshops, and other events must be assigned to timeslots and rooms
while satisfying resource constraints and minimising soft-constraint violations.

The project also studies operational policy changes:

- removing Friday afternoon teaching;
- removing teaching between 17:00 and 18:00;
- applying both restrictions;
- using either 30-minute or 60-minute scheduling intervals.

## My Contribution

I developed the mixed-integer programming models used for the exact optimisation
approach. This included translating the scheduling requirements into decision
variables, hard constraints, soft-constraint penalties, and room-allocation
models.

The simulated-annealing component was developed by another member of the group.

## Methodology

- Mixed-integer programming for event-time and room assignment
- Hard constraints for event clashes, room suitability, and resource capacity
- Penalised soft constraints for timetable quality
- Scenario analysis across teaching hours and timeslot resolutions
- Comparison of exact optimisation with a simulated-annealing heuristic

## Repository Contents

- `OR_Report.pdf` - full project report, methodology, experiments, and findings.
- `BioQuarter_*`, `EasterBush_*`, and `KB_*` notebooks - MIP experiments for
  different campuses, policies, and timeslot lengths.
- `Cleaned *.xlsx` - processed event, programme, and room data.

Notebook names encode the scenario being solved. For example, `30_9to5` denotes
30-minute timeslots with the teaching day restricted to 09:00-17:00.

## Running the Models

Open the notebook for the desired campus and policy scenario. The models require
Python, the optimisation packages imported in the notebook, and the cleaned
Excel input files in the expected relative location.

## Key Skills Demonstrated

Large-scale optimisation, MIP formulation, scenario analysis, data preparation,
room allocation, computational experimentation, and collaborative research.

## Limitations and Further Work

The complete university problem is too large for a single straightforward exact
formulation. Future work could consolidate repeated notebooks into parameterised
modules, strengthen the formulation, and combine exact allocation with adaptive
large-neighbourhood search.

## Academic Context

Group project completed at the University of Edinburgh.
