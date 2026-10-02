 Week 1 - Basic Git, Full Stack & E-Commerce Order Flow Notes
1. Basic Git & Version Control
 Core Concepts:
- Version Control System (VCS): Tracks file revisions and history over time.
- Local vs Remote Repository: Local runs on your personal machine; Remote lives on platforms like GitHub for backup and collaboration.
Essential Commands
- `git init` - Initializes a local repository.
- `git status` - Shows modified, staged, or untracked files.
- `git add <file>` - Stages changes for commit.
- `git commit -m "prefix: message"` - Saves staged changes to commit history.
- `git push origin <branch>` - Uploads local changes to GitHub.
2. Fundamentals of Full Stack Development
Full-stack applications consist of three main layers:
- Frontend (Client-Side): Web browser UI built with HTML, CSS, JavaScript, or frameworks (React/Next.js).
- Backend (Server-Side):Business logic, authorization, and APIs handling business processing.
- Database:Persistent storage layer (PostgreSQL, MongoDB, MySQL).
3. Behind the Scenes: What Happens When an Order Is Placed?
When a user clicks **"Place Order"** on an e-commerce platform, the request travels through several steps across the full stack:
