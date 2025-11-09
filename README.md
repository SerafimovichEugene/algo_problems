# Algo Problems

A collection of algorithm problems from LeetCode and other platforms, solved in TypeScript (and possibly Rust in the future).

## Repository Structure

Each problem is organized in its own folder under the `problems/` directory:

```
problems/
├── two-sum/
│   ├── README.md          # Problem description, approach, and complexity analysis
│   └── solution.ts        # TypeScript solution
└── another-problem/
    ├── README.md
    └── solution.ts
```

## Problem Template

Each problem folder should contain:
- **README.md**: Problem description, approach, time/space complexity
- **solution.ts**: TypeScript implementation
- **solution.rs** (optional): Rust implementation for practice

## How to Add a New Problem

1. Create a new folder in `problems/` with a descriptive kebab-case name
2. Add a `README.md` following this structure:
   - Platform and difficulty
   - Problem description
   - Examples
   - Approach explanation
   - Time and space complexity analysis
3. Add your solution in `solution.ts` (and optionally `solution.rs`)

## Building

```bash
npm install
npm run build
```

## Running Solutions

You can run individual solutions using `ts-node` or compile them first:

```bash
# Install ts-node if needed
npm install -g ts-node

# Run a solution
ts-node problems/two-sum/solution.ts
```

## Example Problems

- [Two Sum](./problems/two-sum/) - LeetCode Easy

