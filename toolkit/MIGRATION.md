# Migration Guide

If you are currently using the AGPL or GPL and wish to migrate to AzTU v2.1, follow these steps.

**Prerequisite:** You MUST be the sole copyright holder of the codebase, or you must have explicit, written consent from every contributor who has written code for the project. 

### Step 1: Commit the new license
Replace your existing `LICENSE` file with the AzTU `LICENSE.md`. 

### Step 2: Update your headers
Run a find-and-replace across your codebase to swap your existing GNU headers with the AzTU headers.

### Step 3: Update package managers
* **Node.js:** Change `"license": "AGPL-3.0"` to `"license": "SEE LICENSE IN LICENSE.md"`
* **Rust:** Change `license = "AGPL-3.0"` to `license-file = "LICENSE.md"`

### Step 4: Add a notice to your users
Include a note in your next release changelog:
> *Notice: We have transitioned our licensing from [Previous License] to the AzTU License v2.1. This maintains our strong copyleft and SaaS-protection philosophy, but uses a simplified, explicit license text. Read the new license in our repository.*
