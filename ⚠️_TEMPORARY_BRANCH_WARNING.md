# ⚠️ TEMPORARY BRANCH WARNING ⚠️

## THIS IS A TEMPORARY COMBINED BRANCH - DO NOT PUSH UPSTREAM!

**Branch:** `temp/combined-local-features`  
**Purpose:** Local use only while waiting for PRs to merge  
**Created:** January 9, 2026

## What This Branch Contains

This branch combines TWO pending pull requests for local testing:

1. **PR #1779** - EV Charger Model Information (`debug/ev-charger-plugin`)
   - Adds model information display for EV chargers
   - Enhanced debug logging

2. **PR #1780** - Phase Envelope Protection (`feature/phase-envelope-protection`)
   - Phase protection for imports and exports
   - Parallel mode remote control limit fixes
   - Comprehensive documentation

## ⚠️ CRITICAL WARNINGS ⚠️

### DO NOT:
- ❌ Push this branch to origin (GitHub)
- ❌ Create a PR from this branch
- ❌ Merge this branch to main
- ❌ Base new work on this branch
- ❌ Commit additional changes to this branch

### ONLY USE FOR:
- ✅ Local testing with both features active
- ✅ Running Home Assistant with combined features
- ✅ Verifying no conflicts between features

## When to Delete This Branch

**DELETE THIS BRANCH when:**
1. Both PRs (#1779 and #1780) have been merged to upstream main
2. You pull the updated upstream main
3. Your local main branch contains both features

**Steps to delete:**
```bash
cd /homeassistant/custom_components/solax_modbus_repo
git checkout main
git pull upstream main
git branch -D temp/combined-local-features
```

## Why This Branch Exists

GitHub PRs must be based on clean branches with only their specific changes. This temporary branch allows local use of both features simultaneously while the PRs are under review.

## Tracking

This temporary branch is tracked in the main HA repository TODO list. See TODO.md for task details.

---

**If you see this file, remember: This is a TEMPORARY branch for LOCAL use only!**

**Never push `temp/*` branches to origin!**

