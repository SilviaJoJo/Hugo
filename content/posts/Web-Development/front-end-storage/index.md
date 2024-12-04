---
title: "SessionStorage vs LocalStorage"
date: 2024-12-03T11:41:17-05:00
description: A comparison of web storage mechanisms SessionStorage and LocalStorage
menu:
  sidebar:
    name: Web Storage
    identifier: web-storage
    parent: web-development
    weight: 10
hero: forest.jpg
tags:
- frontend
- web storage
- javascript
categories:
- web development
---

## SessionStorage vs LocalStorage

### LocalStorage
- **Purpose**: Persistent web storage
- **Function**: 
  - Stores data with no expiration date
  - Persists across browser sessions
  - Shared across browser tabs
- **Key Features**:
  - Data survives browser restarts
  - ~5-10MB storage capacity
  - Same-origin access only
  - Accessible via JavaScript

### SessionStorage
- **Purpose**: Temporary web storage
- **Function**:
  - Stores data for one browser session
  - Clears when tab is closed
  - Isolated per browser tab
- **Key Features**:
  - Tab-specific storage
  - ~5-10MB storage capacity
  - Temporary data persistence
  - Same-origin access only

### Relationship
1. **Common Traits**:
   - Both store key-value pairs
   - Both are web storage APIs
   - Both have similar storage limits
   - Both are vulnerable to XSS attacks

2. **Use Cases**:
   - LocalStorage: User preferences, theme settings, cached data
   - SessionStorage: Form data, page position, temporary session data

3. **Security**:
   - Neither suitable for sensitive data
   - Both require careful XSS protection
   - Both limited to same-origin access

Think of it as:
- LocalStorage is like a persistent notebook
- SessionStorage is like a temporary scratch pad