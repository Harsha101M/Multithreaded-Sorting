# Multithreaded-Sorting
A multi-threaded sorting application in C that implements bubble, insertion, selection, and merge sort algorithms. Features concurrent ascending/descending sorts with mutex locks and step-by-step visualization.

## Features

- Multiple sorting algorithms:
  - Bubble Sort
  - Insertion Sort  
  - Selection Sort
  - Merge Sort
- Multi-threaded implementation for concurrent ascending and descending sorting
- Thread synchronization using mutex locks
- Step-by-step visualization of array states during sorting
- Menu-driven interface

## Getting Started

### Prerequisites

- GCC compiler
- POSIX threads library (pthread)
- Unix-like operating system (Linux, macOS)

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/multi-threaded-sort.git
cd multi-threaded-sort
```

2. Compile the program
```bash
gcc -o sort Multi_Threaded_Sort.c -pthread
```

3. Run the executable
```bash
./sort
```

## Usage

1. Choose a sorting algorithm from the menu:
   - 1: Bubble Sort
   - 2: Insertion Sort
   - 3: Selection Sort
   - 4: Merge Sort
   - 5: Exit

2. Enter the number of elements and their values when prompted

3. The program will display:
   - The original array
   - Step-by-step visualization of the sorting process
   - The final sorted array in both ascending and descending order

## Implementation Details

- Uses POSIX threads for concurrent execution of sorting algorithms
- Mutex locks ensure thread synchronization when accessing shared resources
- Each sorting algorithm is implemented in both ascending and descending order
- For merge sort, the array is split into two sub-arrays that are sorted independently using threads
