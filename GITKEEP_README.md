# .gitkeep Files Explanation

## Why .gitkeep files exist

This template uses `.gitkeep` files in empty directories to ensure the complete folder structure is preserved when the repository is cloned or downloaded.

## What are .gitkeep files?

- **Purpose**: `.gitkeep` is a convention (not a Git feature) to force Git to track empty directories
- **Content**: These files are empty (0 bytes)
- **Naming**: The name `.gitkeep` is arbitrary but widely recognized

## Folder Structure Preservation

The following directories contain `.gitkeep` files to maintain the template structure:

```
concepts/
├── business/.gitkeep
├── design/.gitkeep
├── discussions/.gitkeep
├── gtm/.gitkeep
├── interactions/.gitkeep
├── market/.gitkeep
├── product/.gitkeep
├── quality/.gitkeep
├── research/.gitkeep
├── summaries/.gitkeep
├── ux/.gitkeep
└── spec/
    ├── req/.gitkeep
    └── us/.gitkeep

inputs/.gitkeep
```

## Benefits for Template Users

1. **Complete Structure**: Users get the full folder structure immediately
2. **Clear Organization**: Each role has its designated output directory
3. **No Setup Required**: No need to manually create directories
4. **Consistent Workflow**: Everyone starts with the same structure

## Removing .gitkeep Files

Once you start using the template and add content to directories, you can safely remove the `.gitkeep` files. They are only needed to preserve empty directories in Git.

## Best Practices

- Keep `.gitkeep` files in template repositories
- Remove them once directories contain actual content
- Use meaningful directory names that explain their purpose
- Document the folder structure in your main README 