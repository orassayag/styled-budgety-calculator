# Contributing

Contributions to this project are [released](https://help.github.com/articles/github-terms-of-service/#6-contributions-under-repository-license) to the public under the [project's open source license](LICENSE).

Everyone is welcome to contribute to this project. Contributing doesn't just mean submitting pull requests—there are many different ways for you to get involved, including answering questions, reporting issues, improving documentation, or suggesting new features.

## How to Contribute

### Reporting Issues

If you find a bug or have a feature request:
1. Check if the issue already exists in the [GitHub Issues](https://github.com/orassayag/styled-budgety-calculator/issues)
2. If not, create a new issue with:
   - Clear title and description
   - Steps to reproduce (for bugs)
   - Expected vs actual behavior
   - Browser name and version
   - Screenshots (if applicable)

### Submitting Pull Requests

1. Fork the repository
2. Create a new branch for your feature/fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes following the code style guidelines below
4. Test your changes thoroughly in different browsers
5. Commit with clear, descriptive messages
6. Push to your fork and submit a pull request

### Code Style Guidelines

This project uses vanilla JavaScript ES6 with no build tools. Please maintain consistency with the existing codebase:

**JavaScript:**
- Use ES6 features (arrow functions, const/let, template literals)
- Follow the Module Pattern for code organization
- Use descriptive variable and function names
- Keep functions focused and single-purpose
- Add comments for complex logic

**HTML/CSS:**
- Use semantic HTML5 elements
- Maintain BEM-like class naming for CSS
- Keep CSS organized by sections
- Ensure responsive design principles

Before submitting:
```bash
# Test in multiple browsers
# - Chrome
# - Firefox
# - Safari
# - Edge

# Validate HTML
# Use W3C validator: https://validator.w3.org/

# Check console for errors
# Open browser DevTools and ensure no errors appear
```

### Coding Standards

1. **Code Organization**: Follow the existing three-controller pattern (Budget, UI, Global)
2. **Naming**: Use camelCase for variables and functions
3. **Comments**: Add comments to explain "why", not "what"
4. **Browser Compatibility**: Test in modern browsers (last 2 versions)
5. **No Dependencies**: Keep the project dependency-free (vanilla JS only)

### Adding New Features

When adding new features:
1. Maintain the Module Pattern structure
2. Keep separation of concerns (Budget logic, UI logic, Controller)
3. Ensure features work without external libraries
4. Update documentation if needed
5. Test thoroughly

## Questions or Need Help?

Please feel free to contact me with any question, comment, pull-request, issue, or any other thing you have in mind.

* Or Assayag <orassayag@gmail.com>
* GitHub: https://github.com/orassayag
* StackOverflow: https://stackoverflow.com/users/4442606/or-assayag?tab=profile
* LinkedIn: https://linkedin.com/in/orassayag

Thank you for contributing! 🙏
