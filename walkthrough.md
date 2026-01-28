```markdown
# Walkthrough: Linux File Permissions Update

## Step 1: Check File and Directory Details

Used `ls -la` to view detailed permissions in the `projects/` directory.

The output showed:
- One directory: `drafts/`
- One hidden file: `.project_x.txt`
- Five regular files

Each item had a 10-character string like `-rw-rw-r--`, where:
- `-` = regular file
- `rwx` = read, write, execute
- User/Group/Other have different permissions

## Step 2: Remove Write Access for 'Other'

Only `project_k.txt` had write access for “other” users. I removed it:

```bash
chmod o-w project_k.txt
