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
2. Copy templates from `.templates/` folder or create files manually:
   - `README.md` - Use `.templates/README.md` as a starting point
   - `solution.ts` - Use `.templates/solution.ts` as a starting point
   - `solution.rs` (optional) - Use `.templates/solution.rs` for Rust practice
3. Fill in the problem details, examples, and your solution
4. Test your solution by building and running it

See [CONTRIBUTING.md](./CONTRIBUTING.md) for detailed instructions.

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

