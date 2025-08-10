# GitHub Copilot Instructions for CoreframeApps

## Project Overview

CoreframeApps is a comprehensive bundle of web, mobile, and backend applications designed with a modular architecture. The project follows a structured approach: Product → Web/Android/iOS/Mobile/Server/Services/Deployments.

## Architecture & Structure

- **Multi-platform approach**: Supporting web, Android, iOS, and backend services
- **WordPress foundation**: The project includes WordPress components (see .gitignore)
- **Modular design**: Each platform/service should be independently deployable
- **Scalable architecture**: Designed to handle multiple products and services

## Coding Standards & Conventions

### General Guidelines
- Follow platform-specific best practices (PHP for WordPress, Swift for iOS, Kotlin/Java for Android, etc.)
- Use consistent naming conventions across all platforms
- Implement proper error handling and logging
- Write self-documenting code with clear variable and function names
- Follow SOLID principles and clean code practices

### File Organization
- Keep platform-specific code in clearly separated directories
- Use consistent folder structures within each platform
- Place shared utilities and configurations in common directories
- Follow each platform's standard project structure

### Security Practices
- Never commit sensitive configuration files (wp-config.php, API keys, etc.)
- Use environment variables for configuration
- Implement proper input validation and sanitization
- Follow security best practices for each platform

## Development Workflow

### Version Control
- Use meaningful commit messages following conventional commit format
- Create feature branches for new development
- Keep commits atomic and focused on single changes
- Review .gitignore patterns before committing files

### Testing Approach
- Write unit tests for business logic
- Implement integration tests for API endpoints
- Use platform-appropriate testing frameworks
- Maintain test coverage for critical functionality

### Dependencies
- Document all dependencies in appropriate manifest files (package.json, composer.json, etc.)
- Keep dependencies up to date and secure
- Use version pinning for production deployments
- Prefer well-maintained, popular libraries

## Platform-Specific Guidelines

### WordPress/Web Development
- Follow WordPress coding standards
- Use WordPress hooks and filters appropriately
- Implement proper sanitization and validation
- Use WordPress APIs for database operations
- Ensure mobile responsiveness

### Mobile Development (iOS/Android)
- Follow platform-specific design guidelines (Human Interface Guidelines, Material Design)
- Implement proper offline handling
- Use platform-native UI components when possible
- Optimize for performance and battery life

### Backend Services
- Implement RESTful API design principles
- Use proper HTTP status codes
- Implement rate limiting and authentication
- Document APIs thoroughly
- Design for scalability and fault tolerance

## Common Patterns to Follow

1. **Configuration Management**: Use environment-based configuration
2. **Error Handling**: Implement consistent error handling across platforms
3. **Logging**: Use structured logging with appropriate log levels
4. **Authentication**: Implement secure authentication flows
5. **Data Validation**: Validate all input data
6. **API Design**: Use consistent naming and response formats

## Anti-Patterns to Avoid

1. **Hardcoded Values**: Avoid hardcoding URLs, credentials, or configuration
2. **Platform Mixing**: Don't mix platform-specific code unnecessarily
3. **Large Functions**: Break down complex functions into smaller, testable units
4. **Tight Coupling**: Maintain loose coupling between components
5. **Ignoring Errors**: Always handle errors gracefully

## AI Assistant Guidelines

When working on this project:

1. **Context Awareness**: Consider the multi-platform nature when suggesting solutions
2. **Security First**: Always prioritize security in code suggestions
3. **Platform Standards**: Follow platform-specific conventions and best practices
4. **Documentation**: Include appropriate comments and documentation for complex logic
5. **Testing**: Suggest test cases for new functionality
6. **Performance**: Consider performance implications of suggested changes
7. **Maintainability**: Prioritize code that is easy to read and maintain

## Useful Commands

- `git status` - Check current working directory status
- `composer install` - Install PHP dependencies (WordPress)
- `npm install` - Install Node.js dependencies (web frontend)
- Platform-specific build commands as documented in each module

## Resources

- Keep this file updated as the project evolves
- Document new patterns and decisions as they emerge
- Reference platform-specific documentation for detailed guidelines
- Maintain separate README files for each major component/platform

---

This file should be updated regularly to reflect the current state and needs of the project.