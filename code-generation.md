# 🎯 Code Generation Prompts

Generate high-quality code from specifications with these specialized prompts.

## 📋 Available Prompts

1. [**Basic Function Generator**](#basic-function-generator) - Create custom functions
2. [**Class Generator**](#class-generator) - Generate classes and objects  
3. [**API Endpoint Generator**](#api-endpoint-generator) - Create REST endpoints

---

## 📝 Basic Function Generator

**Perfect for:** Creating utility functions, algorithms, data processing functions

### 🎯 The Prompt

```
You are an expert {language} developer. I need you to create a {type} function that {description}.

Requirements:
- {requirements}
- Follow {language} best practices
- Include proper error handling
- Add comprehensive comments explaining the logic
- Consider edge cases such as {edge_cases}
- Optimize for {optimization_focus}

Please provide:
1. The complete function with clear variable names
2. Usage examples with different scenarios
3. Brief explanation of the approach used

Function specifications:
{specifications}
```

### 🔧 Variables to Replace

- `{language}` - Programming language (Python, JavaScript, Java, etc.)
- `{type}` - Function type (utility, helper, algorithm, etc.)
- `{description}` - What the function should do
- `{requirements}` - Specific requirements and constraints
- `{edge_cases}` - Edge cases to consider
- `{optimization_focus}` - What to optimize for (speed, memory, readability)
- `{specifications}` - Detailed function specifications

### 💡 Example Usage

**Input:**
```
You are an expert Python developer. I need you to create a utility function that calculates compound interest.

Requirements:
- Accept principal amount, annual interest rate, number of years, and compounding frequency
- Follow Python best practices
- Include proper error handling
- Add comprehensive comments explaining the logic
- Consider edge cases such as negative values, zero inputs, and very large numbers
- Optimize for readability and accuracy

Please provide:
1. The complete function with clear variable names
2. Usage examples with different scenarios
3. Brief explanation of the approach used

Function specifications:
- Function name: calculate_compound_interest
- Parameters: principal (float), rate (float), years (int), compounds_per_year (int)
- Return: final amount and interest earned as a tuple
```

### ✨ Expected Output
The AI will provide a complete, well-documented function with error handling, examples, and explanations.

---

## 🏗️ Class Generator

**Perfect for:** Creating data structures, service classes, utility classes

### 🎯 The Prompt

```
Act as a senior {language} developer. Create a {class_type} class named {class_name} that {purpose}.

Class Requirements:
- Properties: {properties}
- Methods: {methods}
- Inheritance: {inheritance}
- Design patterns: {patterns}
- Access modifiers: Use appropriate visibility (private, protected, public)

Additional specifications:
- Include constructor/initializer with parameter validation
- Implement proper encapsulation
- Add docstrings/comments for all public methods
- Consider thread safety if applicable
- Follow SOLID principles
- Include error handling for invalid operations

Please provide:
1. Complete class implementation
2. Usage examples demonstrating all features
3. Unit test examples
4. Brief architectural explanation
```

### 🔧 Variables to Replace

- `{language}` - Programming language
- `{class_type}` - Type of class (data structure, service, utility, etc.)
- `{class_name}` - Name of the class
- `{purpose}` - What the class should accomplish
- `{properties}` - List of properties/attributes
- `{methods}` - List of methods/functions
- `{inheritance}` - Inheritance requirements
- `{patterns}` - Design patterns to use

### 💡 Example Usage

**Input:**
```
Act as a senior Python developer. Create a data structure class named BankAccount that manages bank account operations.

Class Requirements:
- Properties: account_number, balance, account_type, owner_name
- Methods: deposit, withdraw, get_balance, transfer, get_statement
- Inheritance: None (standalone class)
- Design patterns: None required
- Access modifiers: Use appropriate visibility (private, protected, public)
```

---

## 🌐 API Endpoint Generator

**Perfect for:** Creating REST API endpoints, web services, microservice endpoints

### 🎯 The Prompt

```
You are a backend developer specializing in {framework}. Create a {method} API endpoint for {purpose}.

Endpoint Specifications:
- Route: {route}
- HTTP Method: {method}
- Request body: {request_format}
- Response format: {response_format}
- Authentication: {auth_type}
- Validation: {validation_rules}

Requirements:
- Implement proper error handling with meaningful HTTP status codes
- Include input validation and sanitization
- Add comprehensive logging for debugging
- Follow RESTful conventions
- Include rate limiting considerations
- Implement proper security measures
- Add API documentation comments

Please provide:
1. Complete endpoint implementation
2. Request/response examples
3. Error handling scenarios
4. Security considerations
5. Testing approach
```

### 🔧 Variables to Replace

- `{framework}` - Web framework (Flask, Express, Spring Boot, etc.)
- `{method}` - HTTP method (GET, POST, PUT, DELETE)
- `{purpose}` - What the endpoint should do
- `{route}` - URL route path
- `{request_format}` - Expected request body format
- `{response_format}` - Response body format
- `{auth_type}` - Authentication method
- `{validation_rules}` - Input validation requirements

### 💡 Example Usage

**Input:**
```
You are a backend developer specializing in Flask/Python. Create a POST API endpoint for user registration.

Endpoint Specifications:
- Route: /api/v1/users/register
- HTTP Method: POST
- Request body: JSON with username, email, password
- Response format: JSON with user_id, success message, or error details
- Authentication: None (public endpoint)
- Validation: Email format, password strength, username uniqueness
```

---

## 🎯 Tips for Better Results

### ✅ **Do's**
- Be specific about your requirements
- Include your experience level
- Mention the project context
- Specify coding standards
- Include performance requirements
- Ask for explanations

### ❌ **Don'ts**
- Use vague descriptions
- Forget to specify the language
- Omit error handling requirements
- Skip security considerations
- Ignore edge cases

## 🚀 Advanced Usage

### **Combining Prompts**
Use multiple prompts in sequence:
1. Generate basic function
2. Add error handling
3. Optimize performance
4. Add documentation

### **Customization Tips**
- Adjust formality level for your AI
- Add specific coding style preferences
- Include team conventions
- Mention deployment environment

---

**Need more code generation prompts? Check out other categories:**
- [🏗️ Architecture Design](./architecture.md) - For system-level code design
- [🔧 API Development](./api-development.md) - For comprehensive API creation
- [📚 Documentation](./documentation.md) - For code documentation

**[← Back to All Prompts](../PROMPTS_INDEX.md)**
