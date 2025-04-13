# 📦 Semantic Versioning Guide

## 🔢 What is Semantic Versioning?
Semantic Versioning follows the format:

`MAJOR.MINOR.PATCH[-PRERELEASE.TAG]`

**Meaning:**
- **MAJOR**: Major version, incompatible API changes
- **MINOR**: Minor version, backward-compatible new features
- **PATCH**: Patch version, backward-compatible bug fixes and small improvements
- **PRERELEASE**: Optional, indicates pre-release versions (e.g., alpha, beta, rc)
- **TAG**: Optional, additional identifier for pre-release versions
MAJOR: Breaking changes (e.g., API changes that are not backward-compatible)

MINOR: New features, backward-compatible

PATCH: Bug fixes and small improvements

This project uses **Semantic Versioning (SemVer)** to manage releases and Docker images.

## 🔢 Format

Semantic Versioning follows this format:

vMAJOR.MINOR.PATCH[-PRERELEASE.TAG]


### Example Versions:
| Version           | Description                                |
|-------------------|--------------------------------------------|
| `v1.0.0`          | First stable release                       |
| `v1.1.0`          | Backward-compatible new features added     |
| `v1.1.1`          | Backward-compatible bug fixes              |
| `v2.0.0`          | Breaking changes introduced                |
| `v2.0.0-alpha.1`  | Early alpha version (experimental)         |
| `v2.0.0-beta.1`   | Feature-complete but potentially unstable  |
| `v2.0.0-rc.1`     | Release Candidate (ready for final testing)|

---

## ✅ Version Types

| Version Type | When to Bump | Description |
|--------------|--------------|-------------|
| `MAJOR`      | Breaking changes | Incompatible API or functionality changes |
| `MINOR`      | New features     | Backward-compatible new features |
| `PATCH`      | Fixes / tweaks  | Backward-compatible bug or issue fixes |

---

## 🚀 Pre-Release Tags

Pre-release tags help distinguish between unstable or testing versions and final/stable releases.

| Tag     | Purpose                              | Example          |
|---------|--------------------------------------|------------------|
| `-alpha.X` | Initial development/testing        | `v2.1.0-alpha.1` |
| `-beta.X`  | Pre-release, feature complete      | `v2.1.0-beta.1`  |
| `-rc.X`    | Release candidate, almost final    | `v2.1.0-rc.1`    |

Use pre-release tags before pushing the final stable release (`vX.Y.Z`).

---

## 📦 Docker Image Tags

Your Docker images are tagged based on SemVer:

| Docker Tag                | Meaning                        |
|---------------------------|--------------------------------|
| `youruser/ad-api:1.0.0`   | Specific release version       |
| `youruser/ad-api:latest`  | Always points to the latest stable release |
| `youruser/ad-api:rc`      | Latest release candidate       |
| `youruser/ad-api:beta`    | Latest beta version            |

---

## 💡 How to Create a Version Tag

```bash
# Create a tag
git tag -a v1.2.3 -m "Describe the release"

# Push tag to GitHub (triggers CI)
git push origin v1.2.3


```

For pre-releases:
```bash
git tag -a v2.0.0-rc.1 -m "First release candidate"
git push origin v2.0.0-rc.1
```

## Best Practices

- ✅ Start from v0.1.0 if you're still early in development
- ✅ Move to v1.0.0 once stable/public
- ✅ Only bump MAJOR if you introduce breaking changes
- ✅ Add changelogs to each release (manual or automated)

### When using Semantic Versioning, the PATCH version (the last number in vMAJOR.MINOR.PATCH) represents bug fixes and small backward-compatible changes.

But it doesn’t mean:

"1 bug fix = +1 patch version"

Instead, you group fixes into meaningful releases.

✅ Best Practice:
You can fix multiple bugs before tagging a new version.

The key idea is: "Has anything changed in a way that users should know about?"

So, only bump the patch version when you want to release those fixes.

Example Workflow:
You fix 3 small bugs (maybe over a week).

You commit and test them.

When you’re ready to publish the fixes:

bash
Copy
Edit
git tag -a v1.0.1 -m "Fixed 3 minor bugs"
git push origin v1.0.1
This triggers your GitHub Action, runs security checks, builds Docker, and publishes everything tagged v1.0.1.

🧠 TL;DR:
PATCH = safe changes / fixes

You bump it when you're ready to release, not for every single commit

Use changelogs or release notes to describe what was fixed

## 📖 Resources
semver.org
GitHub Releases Docs
