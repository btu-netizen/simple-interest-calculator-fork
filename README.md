# Simple Interest Calculator

This repository contains a Bash script to compute simple interest.

## How to run

```bash
bash simple-interest.sh

### **CODE_OF_CONDUCT.md**  
- Tên file: `CODE_OF_CONDUCT.md`  
- Nội dung: dùng mẫu **Contributor Covenant** hoặc mẫu tiêu chuẩn mà trường / khóa học yêu cầu.

### **CONTRIBUTING.md**  
Mẫu nội dung:

```md
## Contributing Guidelines

To contribute:
1. Fork this repository
2. Create a branch (git checkout -b feature-name)
3. Make changes & commit
4. Push to your fork and open a Pull Request

Please follow code style, write clear commit messages, and test your changes.
#!/bin/bash
# Simple Interest Calculator

echo "Enter Principal:"
read principal
echo "Enter Rate of Interest (per year %):"
read rate
echo "Enter Time in years:"
read time

interest=$(echo "scale=2; $principal * $rate * $time / 100" | bc)
echo "Simple Interest = $interest"
