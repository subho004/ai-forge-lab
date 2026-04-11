# A2A Guide (submodule)

This repository includes the `a2a-guide` submodule at `external/a2a-guide`.

Summary:
- **Location:** `external/a2a-guide`
- **Source:** https://github.com/subho004/a2a-guide
- **Purpose:** Practical Action-to-Action patterns, examples, and documentation for chaining agent actions.

How to initialize after cloning:

```bash
git clone --recursive <repo-url>
cd ai-forge-lab
git submodule update --init --recursive
```

To update the submodule to latest remote:

```bash
cd external/a2a-guide
git pull origin main
cd ../..
git add external/a2a-guide
git commit -m "Update a2a-guide submodule"
```

Where to find details: see [external/a2a-guide](external/a2a-guide)
