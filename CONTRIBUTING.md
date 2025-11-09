# Contributing Guide

## Adding a New Problem

### 1. Create a Problem Folder

Create a new folder in the `problems/` directory with a descriptive kebab-case name:

```bash
mkdir -p problems/problem-name
```

### 2. Use Templates

Copy the template files to your new problem folder:

```bash
cp .templates/README.md problems/problem-name/
cp .templates/solution.ts problems/problem-name/
# Optional: for Rust practice
cp .templates/solution.rs problems/problem-name/
```

Alternatively, you can create the files manually using the template structure below.

### 3. Fill in the README

### 3. Fill in the README

Edit the `README.md` file with your problem details following this structure:

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

### 4. Fill in the TypeScript Solution

Edit the `solution.ts` file with your implementation:

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

### 5. (Optional) Fill in Rust Solution

If practicing Rust, edit the `solution.rs` file with your Rust implementation.

### 6. Test Your Solution

Build and run your solution:

```bash
# Build
npm run build

# Run the compiled solution
node dist/problems/problem-name/solution.js
```

### 6. Update the Main README

### 7. Update the Main README

Add your problem to the list in the main README.md under "Example Problems".

## Best Practices

- Use clear, descriptive variable names
- Add comments for complex logic
- Include time and space complexity analysis
- Test with multiple examples
- Follow TypeScript best practices (use types, avoid `any`)
- Keep solutions clean and readable
