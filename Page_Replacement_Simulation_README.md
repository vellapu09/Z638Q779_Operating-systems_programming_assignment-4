# Page Replacement Algorithms Simulation

This project simulates three different page replacement algorithms: Least Recently Used (LRU), Optimal, and First In First Out (FIFO). The simulation is designed to understand and analyze the performance of these algorithms in terms of the number of page faults that occur during the simulation, given a specific page reference string and a number of frames.

## Algorithms Implemented

- **Least Recently Used (LRU):** Evicts the least recently used page when a page fault occurs and a new page needs to be loaded into a frame.
- **Optimal:** Evicts the page that will not be used for the longest period of time in the future.
- **First In First Out (FIFO):** Evicts the oldest page in the frames based on arrival time.

## Requirements

- Python 3.x

## How to Run the Simulation

1. Ensure you have Python installed on your system.
2. Copy the Python script into a file named `page_replacement_simulation.py`.
3. Open a terminal or command prompt.
4. Navigate to the directory containing `page_replacement_simulation.py`.
5. Run the script using the command:

```bash
python page_replacement_simulation.py
```

## Input

The script uses a predefined page reference string and a specified number of frames as input for the simulation. These are defined at the beginning of the script and can be modified as needed.

Example:
- Page Reference String: `[1, 2, 3, 4, 1, 2, 5, 1, 2, 3, 4, 5]`
- Number of Frames: `4`

## Output

The script outputs the steps of the simulation for each page replacement algorithm, displaying the state of the frames and the number of page faults at each step. It concludes with the total number of page faults for each algorithm.

## Sample Output

For each algorithm, the output will look something like this:

```
Results for LRU Algorithm:
Page fault (1) - Page Table: {1}, Frames: [1], Faults: 1
Page fault (2) - Page Table: {1, 2}, Frames: [1, 2], Faults: 2
...
Total Page Faults: [Total Faults]
```

Replace `[Total Faults]` with the actual number of page faults calculated by the simulation.

## Customization

You can customize the page reference string and the number of frames at the beginning of the script to simulate different scenarios and analyze the performance of each algorithm under various conditions.