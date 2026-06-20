# Text Analyzer

A single-file Java console application that reads a text file and reports statistics about its contents: character and word counts, letter-frequency distribution, shortest/longest word lengths, and the most common uni-grams and bi-grams.

## What it does

Given the path to a text file, the program prints:

- **Character count** (excluding whitespace)
- **Letter frequency** in descending order
- **Word count**
- **Shortest** and **longest** word lengths
- **Top 20 uni-grams** (single words by frequency)
- **Top 20 bi-grams** (adjacent word pairs by frequency)

It demonstrates file I/O (`BufferedReader`), frequency counting with `HashMap`, custom sorting with comparators, and a simple n-gram generator.

## Tech stack

- Java (standard library only — no external dependencies)

## Project structure

```
text-analyzer/
└── src/
    └── TextAnalyzer.java   # main program + helper methods
```

## Build and run

```bash
javac src/TextAnalyzer.java -d out
java -cp out TextAnalyzer
```

When prompted, enter the path to a `.txt` file to analyze:

```
Enter the file path: sample.txt
```

## Notes

The class is in the default package, so it is run as `TextAnalyzer` (no package prefix). All analysis logic lives in static helper methods within the single source file.
