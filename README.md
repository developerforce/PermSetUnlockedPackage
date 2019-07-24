<h1 align="center">Trailhead Packaging Permission Sets Project</h1>
This project contains the sample custom objects and custom tab for the Trailhead project 'Packaging Permission Sets with Salesforce DX'. 

===========================
### Contents:
- [Tool Versioning](#tool-versioning) 
- [Resources](#resources)

===========================
### Tool Versioning
|  Tool:       |  Version:  |
| ------------ | ---------- | 
| **SFDX-CLI** | ![npm](https://img.shields.io/npm/v/sfdx-cli.svg?label=SFDX-CLI&logo=Salesforce&style=Popout)  |

===========================
### The Project Overview

# Set Up the Salesforce DX Project
Our first goal is to set up a developer project which we'll use to modify our application. It starts by cloning the repository. Use the command ...
```
git clone https://github.com/developerforce/sfdx-package-profiles-to-permsets
```
… or ...
```
git clone git@github.com:developerforce/sfdx-package-profiles-to-permsets
```
… to clone the repository. Then, open the directory.
```
  cd sfdx-package-profiles-to-permsets
```
# Authorize Dev Hub in your Trailhead Playground
Log into your Dev Hub org.
```
  sfdx force:auth:web:login -d -a "Hub Org"
  ```
Proceed to log in with your dev hub credentials.

If you already have an authorized Dev Hub, set it as the default:
```
  sfdx force:config:set defaultdevhubusername=<username|alias>
```

# Create a scratch org 
```
  sfdx force:org:create -s -f config/project-scratch-def.json
```

If you want to use an existing scratch org, set it as the default:
```
  sfdx force:config:set defaultusername=<username|alias>
```
# Push the source to your scratch org
```
  sfdx force:source:push
```
# Open the scratch org.
```
    sfdx force:org:open --path one/one.app
```
===========================
### Resources
For details on using sfdx-simple, please review the [Salesforce DX Developer Guide](https://developer.salesforce.com/docs/atlas.en-us.sfdx_dev.meta/sfdx_dev).