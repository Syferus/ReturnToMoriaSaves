# Lord of the Rings: Return to Moria Shared Save Repository

Welcome to the collaborative repository for syncing the shared world save game of Lord of the Rings: Return to Moria. This repository facilitates a seamless synchronization of the world save file among all players, ensuring an updated and synchronized game state for each session.

## Table of Contents

- [Directory Structure](#directory-structure)
- [Branching Strategy](#branching-strategy)
- [.gitignore Configuration](#gitignore-configuration)
- [Contribution Guidelines](#contribution-guidelines)
- [Getting Help](#getting-help)
- [FAQs](#faqs)

## Directory Structure

This section provides information on how to set up the repository on your local machine.

```plaintext
C:\Users\[USERNAMEHERE]\AppData\Local\Moria\Saved\SaveGames
```

- Replace `[USERNAMEHERE]` with your actual username on your PC.

## Branching Strategy

The `main` branch is the canonical branch that hosts the latest stable save game state. Here's how to sync your game before and after a session:

```bash
# Before hosting a session:
git pull origin main

# After playing the session:
git add .
git commit -m "Session update: [DATE]"
git push origin main
```

- Replace `[DATE]` with the actual date of the session.

## .gitignore Configuration

This section provides details on the files excluded from synchronization to prevent overwriting personal character data and individual game settings.

```plaintext
MC_*.sav
Options*.sav
```

## Contribution Guidelines

We welcome suggestions to improve the synchronization process. Here's how you can contribute:

- Open an issue to discuss your suggestion or identify a problem.
- Create a pull request to propose changes to this repository.

## Getting Help

For any queries or issues related to this repository or the save sync process, contact the repository administrator or open an issue.

## FAQs

Answers to frequently asked questions to help users and contributors understand the repository better.

- **Q: How do I back up my character data?**
- **A:** It's the responsibility of individual players to back up their character data locally.

- **Q: What should I do if I encounter a sync issue?**
- **A:** Open an issue on this repository detailing the problem, and we'll work together to resolve it.

Embark on your adventures in Middle-Earth with peace of mind, knowing your shared world remains synchronized!
