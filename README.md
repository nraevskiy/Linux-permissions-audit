# Linux-permissions-audit

This project simulates a security scenario where I updated file and directory permissions to comply with authorization policies using Linux commands.

## Use Case

The research team needed to update access controls for sensitive files. I used Linux tools to:

- Identify existing permission issues
- Restrict unauthorized access
- Ensure directory-level access is user-specific

## Commands Used

```bash
ls -la
chmod o-w project_k.txt
chmod u-w .project_x.txt
chmod g-w .project_x.txt
chmod g+r .project_x.txt
chmod g-x drafts/

