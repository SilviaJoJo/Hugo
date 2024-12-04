---
title: "Running Python Files: Module vs Script"
date: 2024-12-03T11:52:29-05:00
description: Understanding the difference between running Python files as scripts vs modules
menu:
  sidebar:
    name: Python Execution
    identifier: python-execution
    parent: tools
    weight: 10
hero: hero.svg
tags:
- python
- programming
- basics
categories:
- tools
---

## Running Python Files: Script vs Module

### Script Execution
- **Purpose**: Direct program execution
- **Function**:
  - Runs file directly from command line
  - Executes code sequentially
  - `__name__ == "__main__"`
- **Key Features**:
  - Command line usage
  - One-off automation tasks
  - Testing during development

### Module Execution
- **Purpose**: Code reusability
- **Function**:
  - Imported into other Python files
  - Code accessed as library
  - `__name__ == "module_name"`
- **Key Features**:
  - Reusable components
  - Library functions
  - Part of larger applications

### Relationship
1. **Best Practices**:
   ```python
   def main():
       # Main execution code
       pass

   if __name__ == "__main__":
       main()  # Only runs when executed as script
   ```

2. **Use Cases**:
   - Script: Direct execution, CLI tools
   - Module: Library code, reusable functions

3. **Module Command Line**:
   ```bash
   # Run as module
   python -m mymodule
   
   # Run as script
   python script.py
   ```

Think of it as:
- Scripts are like standalone programs
- Modules are like library components