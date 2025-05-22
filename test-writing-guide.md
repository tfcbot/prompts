# Test Writing Guide

## Unit Testing

### 1. Identify Test Scope
- Determine the specific function, module, or component to be tested
- List all expected inputs and outputs for the function
- Document any side effects the function may have

### 2. Test Input Validation
- Write tests to verify the function handles valid inputs correctly
- Write tests to verify the function handles invalid inputs properly (null, undefined, wrong types)
- Include edge cases (empty arrays, minimum/maximum values, boundary conditions)
- Test type validations using Zod when schema metadata is available

### 3. Test Output Validation
- Verify the function returns expected outputs for various inputs
- Test output data structure conforms to expected schema
- Verify all transformations are applied correctly
- Test for correct error handling and appropriate error messages

### 4. Test Performance Requirements
- If applicable, test that the function performs within specified time constraints
- Test memory usage if relevant to the function's requirements

### 5. Setup and Teardown
- Create setup functions to generate test fixtures
- Ensure proper teardown to avoid test pollution
- Use mocks for external dependencies to isolate unit behavior

## Integration Contract Testing

### 1. Identify Contract Boundaries
- Document all integration points between components/services
- Specify the expected request/response formats for each integration point
- Define the behavior contracts between components

### 2. Test Contract Validation
- Verify that components adhere to their defined contracts
- Test that data passed between components maintains integrity
- Verify contract versioning is handled appropriately if applicable

### 3. Test Integration Scenarios
- Develop tests for common integration flows
- Test error handling across component boundaries
- Verify asynchronous communication works as expected

### 4. Mock External Dependencies
- Create realistic mock responses for external systems
- Simulate various response scenarios (success, failure, timeout)
- Test fallback mechanisms when dependencies fail

### 5. Environment Configuration
- Document all environment variables and configuration needed
- Ensure tests can run in isolated environments
- Provide configuration for local, staging, and CI environments

## Implementation Guidelines

1. Use appropriate testing frameworks for your language/platform
2. Organize tests to mirror the structure of your application code
3. Aim for high test coverage but prioritize critical paths
4. Document test setup requirements and procedures
5. Implement continuous integration to run tests automatically
6. Review tests during code reviews
7. Maintain test code with the same standards as production code

## Example Test Structure

```javascript
// Unit test example
describe('functionName', () => {
  // Input validation tests
  test('handles valid inputs correctly', () => {
    // Test implementation
  });
  
  test('rejects invalid inputs', () => {
    // Test implementation
  });
  
  // Output validation tests
  test('returns expected output structure', () => {
    // Test implementation
  });
  
  // Edge cases
  test('handles edge case scenario', () => {
    // Test implementation
  });
});

// Integration contract test example
describe('ServiceAToServiceB integration', () => {
  test('ServiceA sends properly formatted requests to ServiceB', () => {
    // Test implementation
  });
  
  test('ServiceA handles ServiceB responses correctly', () => {
    // Test implementation
  });
  
  test('Contract versioning is respected', () => {
    // Test implementation
  });
});
```

Remember to prioritize readability and maintainability in your tests. Tests serve as documentation of system behavior and should be clear to other developers. 