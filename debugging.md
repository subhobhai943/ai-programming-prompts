# 🐛 Debugging Prompts

Systematic approaches to identify and fix code issues with AI assistance.

## 📋 Available Prompts

1. [**General Code Debugging**](#general-code-debugging) - Fix runtime and logic errors
2. [**Performance Issue Debugging**](#performance-debugging) - Optimize slow code
3. [**Logic Error Debugging**](#logic-error-debugging) - Fix incorrect behavior

---

## 🔍 General Code Debugging

**Perfect for:** Runtime errors, unexpected behavior, crashes, exceptions

### 🎯 The Prompt

```
You are an expert debugger and {language} developer. I'm experiencing {issue_type} with my code.

Problem Description:
- Expected behavior: {expected_behavior}
- Actual behavior: {actual_behavior}
- Error message (if any): {error_message}
- Environment: {environment_details}

Code to debug:
{code_snippet}

Context and constraints:
- {context_information}
- This code is part of: {project_context}
- Dependencies/libraries used: {dependencies}

Please help me:
1. Identify the root cause of the issue
2. Explain why this problem occurs
3. Provide a corrected version of the code
4. Suggest preventive measures to avoid similar issues
5. Recommend debugging techniques for this type of problem
6. Highlight any potential related issues I should watch for

Additional analysis:
- Are there any performance implications?
- Security considerations?
- Best practices violations?
```

### 🔧 Variables to Replace

- `{language}` - Programming language
- `{issue_type}` - Type of issue (runtime error, logic error, performance issue)
- `{expected_behavior}` - What should happen
- `{actual_behavior}` - What actually happens
- `{error_message}` - Exact error message
- `{environment_details}` - OS, versions, etc.
- `{code_snippet}` - The problematic code
- `{context_information}` - Additional context
- `{project_context}` - What type of project this is
- `{dependencies}` - Libraries and frameworks used

### 💡 Example Usage

**Input:**
```
You are an expert debugger and Python developer. I'm experiencing a runtime error with my code.

Problem Description:
- Expected behavior: Function should return the average of a list of numbers
- Actual behavior: Getting "TypeError: unsupported operand type(s) for +: 'int' and 'str'"
- Error message (if any): TypeError: unsupported operand type(s) for +: 'int' and 'str'
- Environment: Python 3.9, running in local development environment

Code to debug:
def calculate_average(numbers):
    total = 0
    for num in numbers:
        total += num
    return total / len(numbers)

# Test data
data = [1, 2, "3", 4, 5]
result = calculate_average(data)
print(result)

Context and constraints:
- Data comes from user input via a web form
- This code is part of: A data analysis web application
- Dependencies/libraries used: Flask, NumPy
```

---

## ⚡ Performance Issue Debugging

**Perfect for:** Slow code, memory issues, CPU bottlenecks, scalability problems

### 🎯 The Prompt

```
Act as a performance optimization expert for {language}. I'm experiencing performance issues with my code.

Performance Problem:
- Current performance: {current_performance}
- Expected/target performance: {target_performance}
- Bottleneck symptoms: {symptoms}
- Testing methodology: {test_conditions}
- Hardware/environment: {system_specs}

Code with performance issues:
{code_snippet}

Additional context:
- Input data characteristics: {data_characteristics}
- Frequency of execution: {execution_frequency}
- Memory constraints: {memory_limits}
- Concurrency requirements: {concurrency_needs}

Please analyze and provide:
1. Performance bottleneck identification
2. Root cause analysis with measurements
3. Optimized code solution
4. Performance comparison (before/after estimates)
5. Alternative approaches to consider
6. Profiling recommendations
7. Monitoring suggestions for production
8. Scalability considerations

Focus areas:
- Time complexity analysis
- Memory usage optimization
- I/O efficiency
- Algorithm improvements
- Data structure optimization
```

### 🔧 Variables to Replace

- `{language}` - Programming language
- `{current_performance}` - Current speed/metrics
- `{target_performance}` - Desired performance
- `{symptoms}` - What you observe (slow, crashes, high CPU)
- `{test_conditions}` - How you're testing
- `{system_specs}` - Hardware and environment details
- `{code_snippet}` - The slow code
- `{data_characteristics}` - Size and type of data
- `{execution_frequency}` - How often code runs
- `{memory_limits}` - Available memory
- `{concurrency_needs}` - Multi-threading requirements

---

## 🧠 Logic Error Debugging

**Perfect for:** Incorrect results, wrong calculations, flawed business logic

### 🎯 The Prompt

```
You are a logic analysis expert specializing in {language}. I have a logic error in my code that's producing incorrect results.

Logic Problem Analysis:
- Function/module purpose: {purpose}
- Expected logic flow: {expected_logic}
- Current incorrect behavior: {incorrect_behavior}
- Test cases that fail: {failing_tests}
- Test cases that pass: {passing_tests}

Code with logic error:
{code_snippet}

Business/domain context:
- Business rules: {business_rules}
- Edge cases to consider: {edge_cases}
- Input constraints: {input_constraints}
- Output requirements: {output_requirements}

Please provide:
1. Step-by-step trace of current logic execution
2. Identification of where logic deviates from requirements
3. Corrected logic with detailed explanation
4. Additional test cases to verify the fix
5. Suggestions to prevent similar logic errors
6. Code review checklist for this type of logic

Analysis approach:
- Trace through the algorithm step by step
- Identify assumption errors
- Check boundary conditions
- Verify mathematical formulas
- Validate business rule implementation
```

---

**Related Prompts:**
- [👁️ Code Review](./code-review.md) - For quality analysis
- [⚡ Performance Optimization](./performance.md) - For speed improvements
- [🧪 Testing](./testing.md) - For creating tests to prevent bugs

**[← Back to All Prompts](../PROMPTS_INDEX.md)**
