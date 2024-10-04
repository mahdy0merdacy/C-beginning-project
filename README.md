# Parallel CSV Processor

This project is a **Parallel CSV Processor** built in C. It is designed to handle large CSV files efficiently by splitting the workload across multiple threads, allowing for faster processing and analysis of data.

## Features

- **Multithreading:** Utilizes multiple threads to process large CSV files in parallel, improving performance on large datasets.
- **Data Filtering:** Apply filters to CSV data based on user-defined conditions.
- **Data Aggregation:** Perform basic aggregation operations like sum, average, max, and min on specific columns.
- **Command-line Interface:** Allows users to specify the input CSV file, output file, and any filtering or aggregation conditions through the command line.

## How It Works

1. The program reads a large CSV file.
2. Data is split into smaller chunks and processed in parallel using `pthread` (POSIX threads).
3. The program can filter and aggregate data based on user inputs, processing the data concurrently for efficiency.

## Setup and Usage

### Prerequisites

- **GCC or Clang:** A C compiler must be installed.
- **POSIX Threads:** The project relies on the POSIX threading library.

### Build

Clone the repository and build the project using the `Makefile`:

```bash
git clone https://github.com/yourusername/parallel-csv-processor.git
cd parallel-csv-processor
make
