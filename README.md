# WSN Bi-objective Dataset

Input instances used in research on network lifetime and target coverage optimization in wireless sensor networks.

## Dataset

The collection contains 30 network instances:

| Instance names | Sensors | Targets | Instances |
|---|---:|---:|---:|
| s10r0–s10r9 | 10 | 121 | 10 |
| s20r0–s20r9 | 20 | 121 | 10 |
| s30r0–s30r9 | 30 | 121 | 10 |

Each instance contains 121 targets arranged on a regular 11 × 11
grid, with equal horizontal and vertical spacing. Sensors are
positioned randomly.

Every sensor has one unit of energy. In the disjoint scheduling
model, each sensor can participate in at most one activation stage.

## File types

- `.txt`: sensor energy capacities and sensor–target coverage lists.
- `.pdf`: visualisation of the corresponding network instance.

Files sharing the same base name describe the same instance.

## TXT file format

The first line contains:

    number_of_targets number_of_sensors

The second line lists the energy capacity of each sensor,
in sensor-index order.

Each subsequent line contains:

    sensor_index covered_target_index covered_target_index ...

For example:

    121 10
    1 1 1 1 1 1 1 1 1 1
    0 104 105 115 116

This example specifies 121 targets and 10 sensors, each having
one unit of energy. Sensor 0 covers targets 104, 105, 115 and 116.

Sensor and target indices start at zero. Target indices range
from 0 to 120. The target identifiers are indices, not coordinates.

A target may appear in several sensor coverage lists.

## Research context

These instances were used in the study:

Amit Dua, Pavel Krömer, Zbigniew J. Czech and Tomasz Jastrząb.
“A Bi-objective Genetic Algorithm for Wireless Sensor Network
Optimization.” Complex, Intelligent and Software Intensive Systems,
2022, pages 147–159.
