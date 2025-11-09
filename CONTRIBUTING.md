# Contributing Guide

## Adding a New Problem

### 1. Create a Problem Folder

Create a new folder in the `problems/` directory with a descriptive kebab-case name:

```bash
mkdir -p problems/problem-name
```

### 2. Create the README

Create a `README.md` file in the problem folder with the following structure:

```markdown
# Problem Name

**Platform:** LeetCode/HackerRank/CodeForces/etc.
**Difficulty:** Easy/Medium/Hard
**Problem Link:** [URL to the problem]

## Problem Description

[Describe the problem clearly]

### Example 1:
\`\`\`
Input: [input]
Output: [output]
Explanation: [explanation]
\`\`\`

### Example 2:
\`\`\`
Input: [input]
Output: [output]
\`\`\`

## Approach

[Explain your approach to solving the problem]

### Time Complexity
- O(?) - [explanation]

### Space Complexity
- O(?) - [explanation]

## Solution

See [solution.ts](./solution.ts) for the TypeScript implementation.
```

### 3. Create the TypeScript Solution

Create a `solution.ts` file:

```typescript
/**
 * Problem Name
 * 
 * Brief description
 */

export function solutionFunction(params: type): returnType {
    // Your solution here
}

// Example usage
if (require.main === module) {
    console.log(solutionFunction(testInput));
}
```

### 4. (Optional) Create a Rust Solution

If practicing Rust, create a `solution.rs` file:

```rust
// Solution in Rust
pub fn solution_function(params: Type) -> ReturnType {
    // Your solution here
}

fn main() {
    println!("{:?}", solution_function(test_input));
}
```

### 5. Test Your Solution

Build and run your solution:

```bash
# Build
npm run build

# Run the compiled solution
node dist/problems/problem-name/solution.js
```

### 6. Update the Main README

Add your problem to the list in the main README.md under "Example Problems".

## Best Practices

- Use clear, descriptive variable names
- Add comments for complex logic
- Include time and space complexity analysis
- Test with multiple examples
- Follow TypeScript best practices (use types, avoid `any`)
- Keep solutions clean and readable
