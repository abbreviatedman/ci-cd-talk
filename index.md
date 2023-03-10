<!-- splash-page -->

# CI/CD

### Continuous Integration and Deployment Explained

---
## Deploying Code In the Modern World

Deploying code is the act of putting it out into the larger world.

This is not simply "saving" the file on a local system anymore!

We'll explore how code is deployed now. But first: how we got here.

---

### The Move To Source Control

30 years ago, developers would simply email code to each other to collaborate.

This has severe issues with syncing up. What if the code doesn't match up? How do you manage who's working on what feature? What if two developers have implemented a feature in different ways?

Whose code is the "source of truth" for the app?

---

### Source Control

Source control is a solution that problem. Also called Version Control, it's a system for tracking changes to a project.

Developers can look at that log of changes to see:

- Which changes were made?
- Who made the changes?
- When were they made?
- Why were those changes needed?

---

### Git

Git is a source control system designed by Linus Torvalds, who also created Linux.

One of its big draws is that it's fully decentralized and distributed.

This means that everyone has their own copy of a project, makes changes, and then puts in a Git request to merge their changes into the project.

Those in charge of the project can then review the changes and, if they approve, automatically merge the changes in.

---

#### Splitting Code Into Branches

The way folks typically work with Git involves "branches".

There are many metaphors for this (including the original "tree branches"), but the "river forks" is helpful.

Sometimes part of a river forks off. And sometimes those forks merge right back together.

---

### Separating Everyone's Code Into Branches

The basic workflow is this:

- A developer "forks" the team project.
- They make the changes they need for the feature they're working on.
- Once they're done, they put in a request to merge the changes back in.
- The team lead looks at the code, runs tests to make sure it works, and merges it back in.
- The developer updates their "fork" with all new changes and starts again.

---

### Other Branches

Besides the main branch and each developer's fork, there are other, specialized branches.

- a "hotfix" branch is often created for quick bug fixes, which can then be merged back into the main branch.

---
### The Release Branch

When the team is ready for a major release, they create a **release branch** to prepare for that. _No new features_ will be added to this release from this point on!

The **release branch** is kept separate from the main branch. Work can be done fixing up and cleaning up the release while, simultaneously, work can be done on the next release.

---

### The Deploy Branch

Once the release is fully ready, it can be merged into the deploy branch.

Then the team can merge this release back into the work they've been doing on the next release, and the cycle begins anew.

---

### What Happens Then?

---

### Old Way

---

#### Test Code

Run the tests and make sure they pass!

---

#### Pre-Deployment Work

- compile the app
- install necessary dependencies
- 


---
#### Deploy

- to web server
- to app store
- to backend server

---

### CI/CD For APIs

---

<!-- splash-page -->
# CI/CD

### Always Be Deploying
