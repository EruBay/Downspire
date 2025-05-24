 Contributing to Downspire

First off, thank you for considering contributing to Downspire! 

## Code of Conduct

This project and everyone participating in it is governed by our Code of Conduct. By participating, you are expected to uphold this code.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues. When creating a bug report, please include:

- **Clear title and description**
- **Steps to reproduce**
- **Expected behavior**
- **Actual behavior**
- **Screenshots if applicable**
- **System information**

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion, please include:

- **Clear title and description**
- **Step-by-step description of the suggested enhancement**
- **Explanation of why this enhancement would be useful**
- **Mockups/examples if applicable**

### Pull Requests

1. Fork the repo and create your branch from `main`
2. Follow the coding standards
3. Write clear commit messages
4. Update documentation as needed
5. Ensure the game builds and runs
6. Submit your pull request

## Coding Standards

### Unity Specific
- Use prefabs for reusable objects
- Follow Unity naming conventions
- Organize assets in logical folders
- Comment complex systems

### C# Style Guide
```csharp
// Good
public class PlayerController : MonoBehaviour
{
    private float moveSpeed = 5f;
    
    void Update()
    {
        HandleMovement();
    }
}

// Bad
public class player_controller : MonoBehaviour {
    private float MoveSpeed = 5f;
    
    void Update(){
        handleMovement();
    }
}
Documentation Standards

Use Markdown for all docs
Include code examples where relevant
Update the changelog
Link between related documents

Questions?
Feel free to open an issue with the "question" label.
