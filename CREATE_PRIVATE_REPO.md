# Creating Nanobot as a Private Repository

This guide explains how to create the nanobot library as a private repository within your account.

## Overview

**nanobot** is an ultra-lightweight personal AI assistant that delivers core agent functionality in just ~4,000 lines of code.

- **Size**: ~3,897 lines of Python code (99% smaller than alternatives)
- **License**: MIT
- **Python**: ≥3.11

## Steps to Create as Private Repository

### 1. Clone the Repository
```bash
git clone http://local_proxy@127.0.0.1:16955/git/cerebrixos-org/nanobot.git
cd nanobot
```

### 2. Create a New Private Repository
On your GitHub account:
1. Go to https://github.com/new
2. **Repository name**: `nanobot` (or your preferred name)
3. **Description**: "Ultra-Lightweight Personal AI Assistant"
4. **Private**: ✓ (Select this option)
5. **Initialize**: Don't initialize with files
6. Click **Create repository**

### 3. Mirror the Repository
```bash
# Remove the original remote
git remote remove origin

# Add your new private repository as the origin
git remote add origin https://github.com/YOUR_USERNAME/nanobot.git

# Push all branches and tags
git push -u origin --all
git push -u origin --tags
```

### 4. Verify the Setup
```bash
git remote -v
# Should show your private repository as origin
```

## Project Structure

```
nanobot/
├── nanobot/              # Main package
├── tests/                # Test suite
├── bridge/               # Bridge components
├── case/                 # Case examples
├── pyproject.toml        # Project configuration
├── Dockerfile            # Docker setup
├── docker-compose.yml    # Docker Compose configuration
├── README.md             # Main documentation
├── SECURITY.md           # Security guidelines
├── LICENSE               # MIT License
└── COMMUNICATION.md      # Community channels
```

## Key Features

- 🐈 Ultra-lightweight design
- ⚡️ ~4,000 lines of code
- 🚀 Fast and efficient
- 🔒 MIT Licensed
- 🤝 Active community

## Getting Started

After creating the private repository:

1. Install dependencies:
   ```bash
   pip install -e .
   ```

2. Run tests:
   ```bash
   pytest
   ```

3. Check the main README.md for more documentation

## Support & Community

- Discord: https://discord.gg/MnCvHqpUGB
- Feishu & WeChat groups (see COMMUNICATION.md)

---

For more information, see the [main README](./README.md) and [Security Guidelines](./SECURITY.md).
