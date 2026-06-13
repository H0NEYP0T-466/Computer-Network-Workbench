# 🤝 Contributing to Computer Network Workbench

Thank you for your interest in contributing to this project! This document provides guidelines and instructions for contributing networking lab exercises and configurations.

---

## 📋 Table of Contents

- [Getting Started](#getting-started)
- [How to Contribute](#how-to-contribute)
- [Lab Naming Conventions](#lab-naming-conventions)
- [Bug Reports & Feature Requests](#bug-requests--feature-requests)
- [Testing Guidelines](#testing-guidelines)
- [Documentation](#documentation)
- [Pull Request Process](#pull-request-process)

---

## 🚀 Getting Started

### Fork & Clone

1. **Fork the Repository**
   - Click the "Fork" button at the top right of this repository
   - This creates a copy of the repository in your GitHub account

2. **Clone Your Fork**
   ```bash
   git clone https://github.com/YOUR_USERNAME/Computer-Network-Workbench.git
   cd Computer-Network-Workbench
   ```

3. **Add Upstream Remote**
   ```bash
   git remote add upstream https://github.com/H0NEYP0T-466/Computer-Network-Workbench.git
   ```

4. **Install Cisco Packet Tracer**
   - Download from [Cisco NetAcad](https://www.netacad.com/courses/packet-tracer)
   - Create a free account if you don't have one
   - Install Packet Tracer for your operating system

---

## 🔧 How to Contribute

### Branch Naming Convention

Create a new branch for your work:

```bash
git checkout -b feature/lab-7-config
# or
git checkout -b fix/lab-3-topology
# or
git checkout -b add/project-vlan-config
```

### Making Changes

1. **Create or modify .pkt files**
   - Open Packet Tracer
   - Create or edit network configurations
   - Save with appropriate naming convention

2. **Add configuration text files** (if applicable)
   - Export device configurations to .txt files
   - Place in appropriate directory

3. **Test your changes**
   - Open the .pkt file in Packet Tracer
   - Verify all devices are properly configured
   - Test connectivity and protocols

4. **Commit your changes**
   ```bash
   git add .
   git commit -m "feat: add VLAN configuration for Lab 7"
   ```

5. **Push to your fork**
   ```bash
   git push origin feature/lab-7-config
   ```

---

## 📝 Lab Naming Conventions

### File Naming

Use the following naming conventions:

- **Regular Labs**: `lab#X.pkt` (e.g., `lab#2.pkt`, `lab#3.pkt`)
- **Date-based Labs**: `DD-mon.pkt` (e.g., `30-apr.pkt`, `7-may-26.pkt`)
- **Lab Tasks**: `DD-mon-labtask.pkt` (e.g., `7-may-labtask.pkt`)
- **General Tasks**: `LABTASK.pkt`
- **Open Ended Labs**: `oel.pkt`
- **Projects**: Place in `PROJECT/` directory with descriptive names

### Configuration Files

- Export device configs as `.txt` files
- Use descriptive names: `switch0.txt`, `router1.txt`, `L2switch.txt`
- Include comments in configurations for clarity

---

## 🐛 Bug Reports & Feature Requests

### Reporting Bugs

If you find an issue with a lab configuration, please create an issue using the bug report template:

1. Go to [Issues](https://github.com/H0NEYP0T-466/Computer-Network-Workbench/issues)
2. Click "New Issue"
3. Select "Bug report"
4. Fill in the required information:
   - **Lab File**: Which .pkt file has the issue
   - **Description**: Clear description of the problem
   - **Steps to Reproduce**: How to trigger the issue
   - **Expected Behavior**: What should happen
   - **Actual Behavior**: What actually happens
   - **Screenshots**: If applicable

### Requesting Features

To request a new lab or feature:

1. Go to [Issues](https://github.com/H0NEYP0T-466/Computer-Network-Workbench/issues)
2. Click "New Issue"
3. Select "Feature request"
4. Describe:
   - **Topic**: What networking topic should be covered
   - **Description**: What the lab should include
   - **Difficulty Level**: Beginner, Intermediate, Advanced
   - **Suggested Devices**: Routers, switches, PCs needed

---

## 🧪 Testing Guidelines

### Testing Your Lab Configurations

Before submitting a pull request:

1. **Open in Packet Tracer**
   - Verify the .pkt file opens without errors
   - Check all devices are present and connected

2. **Verify Configurations**
   - Test IP addressing schemes
   - Verify routing protocols are functioning
   - Check VLAN configurations
   - Test end-to-end connectivity

3. **Document Your Work**
   - Add comments to configurations
   - Include topology descriptions
   - Document any special setup requirements

### Peer Review Checklist

- [ ] Lab opens correctly in Packet Tracer
- [ ] All devices are properly configured
- [ ] Network connectivity is functional
- [ ] Naming conventions are followed
- [ ] No sensitive information is included

---

## 📚 Documentation

### Adding Documentation

When adding new labs:

1. **Update README.md** if adding new lab categories
2. **Add comments** within .pkt files for complex configurations
3. **Include topology diagrams** if helpful (as images or descriptions)

### Configuration Comments

Add comments to device configurations:

```
! Router 1 - Main Gateway
! IP Address: 192.168.1.1/24
! Purpose: Connect LAN to WAN
enable
configure terminal
hostname R1
!
interface GigabitEthernet0/0
 ip address 192.168.1.1 255.255.255.0
 no shutdown
exit
```

---

## 📤 Pull Request Process

1. **Update your branch**
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```

2. **Test thoroughly**
   - Open all modified .pkt files in Packet Tracer
   - Verify configurations work as expected
   - Check for any connectivity issues

3. **Create Pull Request**
   - Go to your fork on GitHub
   - Click "New Pull Request"
   - Fill out the PR template:
     - **Title**: Descriptive title (e.g., "Add Lab 8 - OSPF Configuration")
     - **Summary**: What labs/configurations are included
     - **Testing**: How you tested the configurations

4. **Code Review**
   - Maintainers will review your PR
   - Test configurations in Packet Tracer
   - Address any feedback
   - Make requested changes

5. **Merge**
   - Once approved, your PR will be merged
   - 🎉 Congratulations on your contribution!

---

## 📜 Code of Conduct

Please read our [Code of Conduct](./CODE_OF_CONDUCT.md) before contributing.

---

## ❓ Questions?

If you have questions or need help:

- Open a [Discussion](https://github.com/H0NEYP0T-466/Computer-Network-Workbench/discussions)
- Check existing [Issues](https://github.com/H0NEYP0T-466/Computer-Network-Workbench/issues)

---

**Thank you for contributing! 🎉**
