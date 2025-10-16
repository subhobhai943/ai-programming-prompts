# 👁️ Code Review Prompts

Comprehensive code analysis and quality assessment prompts for better code.

## 📋 Available Prompts

1. [**Comprehensive Code Review**](#comprehensive-code-review) - Complete quality analysis
2. [**Security-Focused Review**](#security-focused-review) - Security vulnerability assessment
3. [**Architecture Review**](#architecture-review) - Design and architecture analysis

---

## 📊 Comprehensive Code Review

**Perfect for:** Pre-production reviews, code quality checks, team code reviews

### 🎯 The Prompt

```
Act as a senior code reviewer and {language} expert. Please conduct a thorough code review of the following code.

Code to review:
{code_snippet}

Context:
- Purpose: {code_purpose}
- Target environment: {environment}
- Performance requirements: {performance_reqs}
- Team coding standards: {coding_standards}
- Project phase: {project_phase}

Review criteria - please analyze each area:

**1. Code Quality & Style:**
- Naming conventions and clarity
- Code organization and structure
- Commenting and documentation
- Adherence to language conventions

**2. Functionality & Logic:**
- Correctness of implementation
- Edge case handling
- Error handling completeness
- Business logic accuracy

**3. Performance & Efficiency:**
- Algorithm efficiency
- Memory usage
- I/O operations optimization
- Scalability considerations

**4. Security:**
- Input validation and sanitization
- Authentication and authorization
- Data protection measures
- Vulnerability assessments

**5. Maintainability:**
- Code modularity and reusability
- Dependency management
- Testing considerations
- Future modification ease

**6. Best Practices:**
- Design pattern usage
- SOLID principles adherence
- Framework-specific best practices
- Industry standards compliance

Please provide:
1. Overall assessment score (1-10)
2. Detailed findings for each area
3. Specific recommendations with examples
4. Priority ranking of issues (Critical/High/Medium/Low)
5. Refactored code examples for major issues
6. Positive aspects worth highlighting
```

---

## 🛡️ Security-Focused Review

**Perfect for:** Security audits, vulnerability assessments, compliance checks

### 🎯 The Prompt

```
You are a cybersecurity expert specializing in secure {language} development. Perform a security-focused code review on the following code.

Code for security analysis:
{code_snippet}

Security context:
- Application type: {app_type}
- Data sensitivity level: {data_sensitivity}
- User access level: {user_access}
- Network exposure: {network_exposure}
- Compliance requirements: {compliance_reqs}

Security review checklist:

**Input Validation & Sanitization:**
- User input validation
- SQL injection prevention
- XSS prevention
- Command injection protection
- Path traversal prevention

**Authentication & Authorization:**
- Authentication mechanisms
- Session management
- Access control implementation
- Privilege escalation risks

**Data Protection:**
- Sensitive data handling
- Encryption implementation
- Data transmission security
- Storage security measures

**Error Handling:**
- Information disclosure in errors
- Logging security considerations
- Exception handling security

**Configuration & Dependencies:**
- Secure configuration practices
- Third-party library vulnerabilities
- Environment variable handling
- Secret management

**Common Vulnerabilities:**
- OWASP Top 10 compliance
- Race conditions
- Buffer overflows (if applicable)
- Cryptographic issues

Provide:
1. Vulnerability assessment (Critical/High/Medium/Low)
2. Specific security issues found
3. Exploit scenarios for each issue
4. Remediation steps with secure code examples
5. Security best practices recommendations
6. Compliance gaps (if any)
7. Security testing recommendations
```

---

## 🏗️ Architecture Review

**Perfect for:** System design analysis, scalability assessment, architectural decisions

### 🎯 The Prompt

```
You are a software architect and {language} expert. Please review this code from an architectural and design perspective.

Code/component to review:
{code_snippet}

Architectural context:
- System role: {system_role}
- Integration points: {integrations}
- Scalability requirements: {scalability_needs}
- Architecture pattern: {architecture_pattern}
- Design constraints: {design_constraints}
- Team size and structure: {team_context}

Architecture review areas:

**Design Principles:**
- SOLID principles adherence
- DRY (Don't Repeat Yourself) compliance
- KISS (Keep It Simple, Stupid) principle
- Separation of concerns
- Loose coupling, high cohesion

**Structural Analysis:**
- Component responsibilities clarity
- Abstraction levels appropriateness
- Interface design quality
- Dependency relationships
- Module organization

**Scalability & Performance:**
- Horizontal scaling readiness
- Vertical scaling considerations
- Performance bottleneck identification
- Resource utilization efficiency
- Caching strategy implementation

**Maintainability:**
- Code complexity assessment
- Testing strategy alignment
- Documentation completeness
- Refactoring ease
- Technical debt identification

**Integration Design:**
- API design quality
- Error propagation handling
- Transaction management
- Data consistency approaches
- Communication patterns

**Future-Proofing:**
- Extensibility considerations
- Technology evolution readiness
- Migration path planning
- Backward compatibility

Provide:
1. Architectural assessment summary
2. Design principle compliance analysis
3. Scalability and performance evaluation
4. Maintainability score and rationale
5. Integration quality assessment
6. Recommended improvements with rationale
7. Alternative architectural approaches
8. Migration/refactoring roadmap (if needed)
```

---

**Related Prompts:**
- [🔒 Security Analysis](./security.md) - For detailed security audits
- [⚡ Performance Optimization](./performance.md) - For performance improvements
- [🔄 Refactoring](./refactoring.md) - For code improvement strategies

**[← Back to All Prompts](../PROMPTS_INDEX.md)**
