### ✅ **Your Expectations / Commands Recap:**

1. **You are using:**
    
    - ✅ `xUnit` for unit testing
        
    - ✅ `NSubstitute` for mocking
        
2. **Test Structure / Style:**
    
    - Must follow your **office convention**, including:
        
        - Clear test method naming
            
        - Region blocks for grouping test cases
            
        - Clear `Arrange`, `Act`, `Assert` pattern
            
        - Only **minimal required properties** used from DTOs/models
            
        - No random assumptions — ask for missing models explicitly
            
3. **You have a `BaseTest` class** that initializes:
    
    - `_sessionMock`, shared setup, etc.
        
    - `ExamWrittenQuestionServiceBaseTests` inherits from it and initializes:
        
        - `_examWrittenQuestionDaoMock`
            
        - `_examDaoMock`
            
        - `_loggerMock`
            
        - `_sut` (the service under test)
            
4. **What you’ve asked me repeatedly:**
    
    - ❌ Do **not** assume unknown DTO/model structure
        
    - ✅ If I don’t know a model, I **must ask for it first**
        
    - ❌ Do **not** use all model properties in tests — just a few relevant ones
        
    - ✅ All code paths (try, catch, logging, etc.) must be **covered**