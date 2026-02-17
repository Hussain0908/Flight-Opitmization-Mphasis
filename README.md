# Airlines Flight Schedule Optimization with Simulated Quantum Annealing

This project provides a solution for the problem of re-accommodating impacted passengers due to airline flight schedule changes. Airlines often need to adjust their flight schedules for reasons such as seasonality, new routes, changes in flight timings, cancellations, and more. The goal is to analyze the impact of these changes on passengers and automatically identify the most suitable alternate flights for them.

## Problem Overview

When airlines modify their flight schedules, passengers may be impacted by cancellations, changes to flight numbers, or re-routing. It is important for the airline to ensure that affected passengers are re-accommodated in an optimal way to reduce customer dissatisfaction. The process involves:

Due to the scale and complexity of this problem, **mathematical optimization** and advanced computational techniques are often employed in the airline industry.

## Solution Overview

This project implements a solution for the above problem using a **Simulated Quantum Annealing** approach to solve the optimization problem. The solution is based on the following key components:

1. **Identification of Impacted Flight Segments and Passengers**: A method to identify the flight segments and passengers that are impacted by schedule changes.
2. **Passenger CVM Score Calculation**: The passenger's CVM score is pre-calculated as part of the input data, which is used for decision-making in the optimization process.
3. **Ranking of Alternative Flights**: A technique to rank alternative flights based on various parameters (e.g., travel time, comfort, etc.).
4. **Optimal Assignment**: Using optimization techniques, the impacted passengers are reassigned to the best possible alternative flights.
5. **Benchmarking**: The solution is benchmarked against a classical optimization approach to assess the efficiency and performance of the quantum-based approach.

### Quantum Approach

We apply **Simulated Quantum Annealing** using **D-Wave's DMO** and **Neal** to model the optimization problem. These quantum techniques allow for the exploration of solution spaces in a way that is expected to be faster than classical approaches, particularly in large and complex instances.

### Classical Approach

In addition to the quantum-based solution, a classical solution is also provided for benchmarking purposes. The classical solution uses traditional optimization techniques to compare performance, such as speed and accuracy, against the quantum annealing approach.

## Key Features

- **Impact Assessment**: Automatically identifies affected passengers and flight segments.
- **Passenger Reaccommodation**: Reassigns passengers to the best available flights based on various factors.
- **Quantum Annealing Implementation**: Utilizes quantum-based optimization using D-Wave's DMO and Neal for fast solution finding.
- **Classical Benchmarking**: Provides a classical baseline to evaluate the quantum solution's performance.
- **Scalable**: Designed to handle large datasets and complex airline scheduling problems.

## Example Results and Visualization

Once the optimization is complete, you can visualize the comparison between the **Quantum Annealing** and **Classical Optimization** approaches. The following table and chart illustrate the **CVM Score** and **Re-accommodation Score** for impacted passengers and the corresponding flight assignments.

### Sample Data (Output)

Here’s an example of the data output from both methods, showing how the quantum and classical methods compare in terms of the assignment quality:

| Flight ID | Passenger ID | Original Flight | New Flight | CVM Score | Re-accommodation Score |
|-----------|--------------|-----------------|------------|-----------|------------------------|
| 123       | 001          | A1              | B2         | 75        | 95                     |
| 124       | 002          | A2              | C1         | 80        | 92                     |
| 125       | 003          | B1              | A2         | 85        | 90                     |
| 126       | 004          | C1              | D2         | 70        | 88                     |
| 127       | 005          | D1              | E1         | 65        | 85                     |

## Disclaimer

**Data Sharing Restrictions:**

The data used in this project pertains to **airline operations** and is subject to strict company policies and confidentiality agreements. As a result, **the actual datasets used in this project cannot be shared or uploaded to GitHub**.

If you wish to implement this solution within your organization or require similar data for testing purposes, please ensure you obtain the appropriate permissions and adhere to your organization’s data privacy policies.

