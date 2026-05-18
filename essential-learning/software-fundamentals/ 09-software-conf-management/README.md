# Software Configuration Management (SCM)

## Introduction

Tom, Katie, and Bob are TV reporters working for a live news channel.  
They live in different cities and use a common online document template to update city news.

All of them edit the same document simultaneously.  
When Tom saved his version, the earlier version saved by Katie got overwritten.  
Similarly, whenever one reporter saved the document, the others’ changes were lost.

This type of issue can also happen in software development projects.

---

# Problem in Software Development

Software development contains many configuration items such as:

- SRS Documents
- Design Documents
- Source Code
- Test Reports
- User Manuals

These items are accessed and modified by multiple team members who may work:

- From different locations
- In different offices
- Across different time zones

If changes are not managed properly:

- Data may get overwritten
- Older versions may be lost
- Conflicts may occur
- Final software quality may be affected

---

# Solution: Software Configuration Management (SCM)

Software Configuration Management helps in:

- Managing changes
- Controlling versions
- Tracking modifications
- Avoiding overwriting issues
- Maintaining consistency in software projects

SCM ensures that all changes made to configuration items are:

- Controlled
- Recorded
- Managed properly

---

# Configuration Items

Configuration items are the important project artifacts that need management.

Examples include:

1. SRS Documents
2. Design Documents
3. Source Code
4. Test Cases
5. Test Reports
6. User Manuals

---

# Need for SCM

SCM is important because:

- Multiple developers work together
- Changes happen frequently
- Different versions must be maintained
- Team coordination is required
- Product quality must be protected

---

# Benefits of SCM

## Advantages

- Prevents data loss
- Maintains version history
- Supports teamwork
- Helps in tracking changes
- Improves software quality
- Reduces conflicts between developers

---

# Real-Time Example

Suppose three developers are working on the same source code file.

Without SCM:
- One developer’s changes may overwrite another’s work.

With SCM:
- Every change is tracked separately.
- Versions are maintained.
- Conflicts can be resolved properly.

---

# Conclusion

Software Configuration Management is an important process in software engineering.

It helps organizations:
- Control software changes
- Maintain document versions
- Coordinate team activities
- Protect project quality

SCM ensures smooth collaboration among team members working on the same project.

# Software Configuration Management (SCM)

# Objectives

After completing this module, you will be able to:

- Define Software Configuration Management
- Explain the importance of SCM
- Define configuration items
- Describe the 4 components of Configuration Management
- Define Check-In and Check-Out from repository
- Explain Change Management
- Explain the importance of Version Management
- Learn about SCM tools

---

# Introduction to SCM

In software development, many team members work together on the same project files.

For example:

- Documents
- Source Code
- Design Files
- Test Reports

When multiple people modify the same file simultaneously, confusion and overwriting problems may occur.

Software Configuration Management (SCM) helps to manage and control these changes properly.

---

# Example Scenario

Two employees are working on the same project document named `abcBank.doc`.

## Step 1

Both employees access the same file from the server.

- Employee 1 updates the document.
- Employee 2 also updates the document.

---

## Step 2

Both employees upload the modified file back to the server.

Problem:
- One person's changes overwrite the other's work.

---

## Step 3

The next day, another employee opens the file and notices that many changes are missing.

This happens because:
- Multiple users modified the same file simultaneously.

---

# Solution to the Problem

The best solution for handling such issues is:

# Software Configuration Management (SCM)

SCM helps teams:
- Track changes
- Control versions
- Avoid overwriting
- Maintain software consistency

---

# What is Software Configuration Management?

A configuration is the functional and physical characteristics of hardware or software defined in technical documentation.

SCM coordinates software development activities by:

- Identifying changes
- Modifying software properly
- Controlling software updates

---

# Activities of SCM

SCM activities include:

1. Identifying changes
2. Controlling changes
3. Ensuring proper implementation of changes
4. Reporting changes to team members

---

# Why Software Configuration Management is Important

## Reasons

### 1. Complex Projects
Most IT projects are large and complex.

### 2. Multiple Team Members
Many developers update code in the repository.

### 3. Code Conflicts
Changes by multiple developers may create conflicts.

### 4. Communication Gap
Without proper management, communication issues occur.

### 5. Better Solution
SCM provides a structured solution for handling changes.

---

# Software Evolution

Software systems continuously evolve due to:

- Different operating systems
- Different machine environments
- New functionality
- User-specific requirements

SCM manages these evolving systems effectively.

---

# Responsibilities of SCM

SCM is responsible for:

- Managing software changes
- Controlling versions
- Reducing development cost and effort
- Supporting team collaboration

---

# Software Entities Managed by SCM

SCM manages different software entities such as:

- SRS Documents
- Design Documents
- Programs
- Test Data
- User Documentation
- Source Code
- Executable Files
- Libraries
- Support Tools

---

# Effective SCM

SCM is effective when:

- Every work product is accounted for
- Every change can be tracked
- All modifications are controlled properly

---

# Software Configuration Management Plan

SCM planning starts during the early phase of the project.

---

## SCM Plan Defines

### 1. Artifacts to Manage
Documents, code, and files to be maintained.

### 2. Responsibilities
Who manages SCM activities.

### 3. Baselines
Creation and maintenance of baselines.

### 4. Change Policies
Rules for change control and version management.

### 5. Records Maintenance
SCM records to be stored properly.

---

# Configuration Item (CI)

A Configuration Item is:

> An aggregation of hardware, software, or both treated as a single entity in the configuration management process.

---

## Important Points

- Large projects create thousands of documents.
- Every document should have a unique name.
- Some documents must be maintained throughout the software life cycle.

---

# Components of SCM

There are 4 major components of SCM:

---

## 1. Configuration Identification

Defines:
- Product
- Configuration documents
- Naming conventions

---

## 2. Change Management

Controls changes made to:
- Product
- Configuration documents

---

## 3. Configuration Status Accounting

Provides:
- Status information
- Change history
- Product configuration details

---

## 4. Configuration Audits

Ensures:
- Quality
- Correctness
- Compliance with standards

---

# Types of Configuration Objects

There are two types:

1. Base Object
2. Aggregate Object

---

# Base Object

A Base Object is:

> The basic unit created during analysis, design, coding, or testing.

## Examples

- Requirement specification section
- Source code module
- Test cases

---

# Aggregate Object

An Aggregate Object is:

> A collection of base objects and other aggregate objects.

## Example

A Design Specification may include:

- Data Design
- Architectural Design
- Module Design
- Interface Design

---

# Baseline

A Baseline is:

> A formally reviewed and approved specification or product that serves as the basis for future development.

Changes to a baseline can only be made using formal change control procedures.

---

# Examples of Baselines

## Baseline A
API structure is completely defined.

## Baseline B
All data access methods are implemented and tested.

## Baseline C
GUI is fully implemented.

---

# Types of Baselines

As software evolves, different baselines are created:

- Developmental Baseline
- Functional Baseline
- Product Baseline

---

# Version Naming Scheme

Common version naming examples:

- 2.0
- 3.01a
- 1.8.5

Example breakdown of `1.8.5`:

- Release Number
- Version Number
- Revision Number

---

# Configuration Repository

All configuration management information is stored in a:

# Repository

---

## Repository Helps Answer Questions Like

- Who has a particular version?
- Which platform is needed?
- Which versions are affected by changes?
- How many faults exist in a version?

---

# Check-In and Check-Out

Configuration items are usually read-only by default.

---

## Check-Out

Developers check out objects so they can modify them.

---

## Check-In

Check-in is:

- Making updated versions available to others
- Saving a new version in the database

---

# Change Management

Change Management controls software modifications systematically.

---

# Activities in Change Management

1. Filtering changes
2. Managing change processes
3. Reviewing Requests for Change (RFC)
4. Reporting management information

---

# Advantages of SCM

- Prevents data loss
- Tracks changes
- Supports teamwork
- Controls software versions
- Reduces conflicts
- Improves software quality

---

# Conclusion

Software Configuration Management (SCM) is an essential process in software engineering.

It helps teams:

- Manage software changes
- Track versions
- Maintain repositories
- Coordinate development activities
- Improve software quality

SCM ensures smooth and controlled software development in team environments.


# Synchronization Control

Synchronization Control helps prevent conflicts when multiple developers work on the same configuration object.

---

## Purpose of Synchronization Control

- Ensures that parallel changes made by different developers do not overwrite each other.
- Locks the object in the project database while one developer is editing it.
- Prevents updates until the checked-out version is returned.

---

# Working of Synchronization Control

## Process Flow

1. Developer checks out the configuration object.
2. Access control locks the object.
3. Developer modifies the extracted version.
4. Modified object is checked in.
5. Database gets updated with the new baseline version.
6. Lock is released for other developers.

---

# Change Control Board (CCB)

## Definition

Change Control Board (CCB) or Software Change Control Board (SCCB) is a committee responsible for deciding whether proposed software changes should be accepted or rejected.

---

## Members of CCB

The board usually consists of:

- Project stakeholders
- Team representatives
- Project managers
- Technical experts

---

## Responsibilities of CCB

- Evaluate proposed changes
- Approve or reject changes
- Ensure controlled implementation
- Maintain project stability

---

## Important Point

The authority of the CCB may vary between projects, but its decisions are generally considered final and binding.

---

# Change Control Process

The change control process ensures that software changes are properly managed.

---

## Steps in Change Control Process

### 1. Request for Change
A request for modification is submitted.

### 2. Impact Analysis
The effects of the change are analyzed.

### 3. Approve / Deny
The change request is either approved or rejected.

### 4. Implement Change
Approved changes are implemented and tested.

### 5. Review and Reporting
Final review and documentation are completed.

---

# Detailed Change Workflow

## Evaluation Phase

- Identify and submit change request
- Evaluate impacts of the change
- Approve or reject the request

---

## Resolution Phase

- Plan the change
- Implement the change
- Test the modifications

---

## Verification Phase

- Verify whether the change works correctly
- Reopen if issues exist
- Close the request if approved

---

# Version Management

## Definition

Version control is a mechanism used to manage multiple versions of files and programs.

---

## Features of Version Management

It allows users to:

- Lock files so only one person edits at a time
- Track changes made to files
- Restore previous versions
- Store historical project data

---

## Advantages

- Instant recall of previous work
- Easy collaboration among developers
- Read-only access to old versions
- Safe modification of files

---

# Benefits of Version Management

## 1. Rollback Support
Return to older versions if errors occur.

## 2. Compare Versions
Highlight differences between file versions.

## 3. Branching Support
Allows parallel development using branches.

## 4. Audit Trail
Maintains records of:
- Modified date
- Modifier name
- Version history
- Metadata

---

# SCM Tools

SCM tools support:

1. Concurrency Management
2. Version Control
3. Synchronization

---

# Popular SCM Tools

## 1. RCS (Revision Control System)

### Features

- Local repository model
- Independent revision storage
- Supports:
  - Revising documents
  - Committing changes
  - Merging files

---

## 2. ClearCase

### Features

- Controlled access to software assets
- Parallel development support
- Workspace management
- Baseline management
- Secure version management
- Reliable build auditing
- Supports large repositories and binary files

---

## 3. Subversion (SVN)

### Features

- Open-source centralized repository
- Allows reverting to previous versions
- Supports concurrent development

---

# Important SCM Terms

| Term | Meaning |
|------|----------|
| Repository (Repo) | Database where files are stored |
| Server | System storing the repository |
| Client | System connected to the server |
| Working Copy | Local copy where changes are made |
| Trunk / Main | Primary development line |
| Add | Adding a new file to the repository |

---

# More SCM Terms

| Term | Meaning |
|------|----------|
| Revision | Version number of a file |
| Head | Latest revision in repository |
| Check Out | Download file for local editing |
| Check In | Upload modified file back to repository |
| Check-In Message | Description of changes made |

---

# Check-In and Check-Out Example

## Basic Check-Ins

Each new check-in creates a new revision:

- r1
- r2
- r3
- r4

Example:
- Milk
- Milk + Eggs
- Milk + Eggs + Juice
- Milk + Eggs + Soup

---

## Check-Out and Edit

- Developers check out the latest revision.
- Changes are made in the working copy.
- Updated files are checked in again.

---

# Diff and Conflict

## Diff

Diff shows the differences between two versions of a file.

Example:
- Added Juice
- Removed Eggs
- Added Soup

---

## Conflict

Conflicts occur when:
- Two developers modify the same section simultaneously.

Example:
- One developer removes Eggs
- Another developer changes Eggs to Cheese

Result:
- SCM identifies conflict
- Manual resolution is required

---

# Branch and Merge

## Branching

Branching creates separate development paths for new features.

Example:
- Main project continues normally
- Separate branch adds Rice feature

---

## Merging

Merging combines branch changes back into the main trunk.

Example:
- Bread added in main branch
- Rice added in feature branch
- Both merged into final version

---

# SCM Activities

## Typical SCM Workflow

1. Store code in a common repository
2. Developers create working copies
3. Developers modify files locally
4. Changes are committed
5. Repository checks for conflicts
6. Merge conflicts if required
7. Check in the final updated version

---

# Additional Advantages of SCM

- Maintains complete history of changes
- Tracks:
  - What changed
  - Why it changed
  - Who changed it
  - When it changed
- Simplifies software maintenance
- Improves collaboration

---

# Conclusion

Software Configuration Management (SCM) is essential for modern software development.

It helps teams:

- Control software versions
- Manage parallel development
- Track changes efficiently
- Avoid conflicts
- Improve collaboration and software quality

SCM ensures reliable and organized software development throughout the project life cycle.
