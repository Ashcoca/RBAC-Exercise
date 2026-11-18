# RBAC-Exercise

Everything in this exercise follows from three ideas in the lecture:

- **RBAC** (Role-Based Access Control): people get roles, roles get permissions. You never grant a person access directly, you grant it to the role.

- **Principle of Least Privilege**: every permission must earn its place. Access you can't justify is access you shouldn't have.

- **Default Deny**: anything the matrix doesn't explicitly allow is denied. Access is designed, not assumed.

## Part 1. Pick a System

Choose **one** system that everyone in the group knows well enough to argue about:

1. **A hospital records system.** Doctors, nurses, patients, billing staff, and at least one person nobody planned for.

2. **A university course platform.** Students, instructors, teaching assistants, registrars, and grades nobody should see early.

3. **A product your own team builds.** Real is better than hypothetical, but only if the whole group knows it.

Write the system name at the top of your board (or file if you're on your computer). List 6 to 10 kinds of people who touch it. Don't design roles yet, just name the people.


## Part 2. Design the roles

Turn your list of people into **roles**. Rules for good roles:

- A role is a **job**, not a person. "Attending Physician" works. "Ash" does not.

- A role bundles permissions. If two roles always have exactly the same permissions, they're one role.

- Aim for **4 to 6 roles**. More than that usually means you're designing around individuals instead of jobs.

- Name roles the way a job posting would. The name should let a newcomer guess roughly what it can do.

While you design roles, also list the **permissions** the system needs. Permissions are verbs on things: view a chart, edit a grade, approve an expense, export a report, delete an account. Write each permission on the board as a short phrase.

## Part 3. Build the matrix

Draw the grid: roles across the top, permissions down the side. Mark each cell **allow** or leave it **deny** (blank). 

Two rules:

1. **Default deny.** You only mark allows. Everything blank is denied, on purpose.

2. **Justify every allow.** For each check mark, your group should be able to finish this sentence out loud: "A [role] needs to [permission] because [reason]." If you can't finish the sentence, blank the cell.


|   | Role 1 | Role 2 | Role 3 | Role 4 |
| --- | --- | --- | --- | --- |
| View patient chart | ✓ | ✓ |   |   |
| Edit patient chart |   |   |   |   |
| ... |   |   |   |   |

(This is a template, not advice. Use your own roles and permissions.)

Expect disagreements. Two group members wanting different permissions in the same cell is the exercise working, not failing. Write your best-resolved version, and keep a one-line note of anything you argued about, because you'll present it.

## Part 4. Present (3 minutes per group)

Each group presents:

1. The matrix, briefly. Name the roles and the shape of the permissions.

2. **Two allows you defended hardest**, with the reason.

3. **One thing the group argued about** and how you settled it.


Keep it under three minutes. The audience's job during each presentation: listen for an allow they'd challenge. Make them defend their roles!
