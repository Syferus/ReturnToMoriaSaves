```markdown
# Lord of the Rings: Return to Moria Shared Save Repository

Welcome to the shared save game repository for Lord of the Rings: Return to Moria! This repository facilitates the synchronization of the world save game file among all players, ensuring a coherent and updated game state for every session.

## Directory Structure

Ensure that this repository is cloned or initialized in the designated directory on your PC:

```plaintext
C:\Users\[USERNAMEHERE]\AppData\Local\Moria\Saved\SaveGames
```

Replace `[USERNAMEHERE]` with your actual username.

## Branching Strategy

The `main` branch is the canonical branch containing the most recent stable save game state. The host for the night's session should pull the latest changes from the `main` branch before starting the game:

```bash
git pull origin main
```

After the session, the host should commit and push the updated world save back to the `main` branch to ensure synchronization with all players:

```bash
git add .
git commit -m "Session update: [DATE]"
git push origin main
```

Replace `[DATE]` with the actual date of the session.

## .gitignore Configuration

The `.gitignore` file is configured to exclude certain files from being tracked by Git to ensure only the world save file is synced among players. The following files are excluded:

```plaintext
MC_*.sav
Options*.sav
```

This setup ensures personal character data and individual game settings are not overwritten.

## Contribution

While the primary goal of this repository is to sync the world save, any suggestions to improve the synchronization process are welcome. Feel free to open an issue or contact the repository administrator.

## Contact

For any queries or issues related to this repository or the save sync process, please contact the repository administrator or open an issue here.

Embark on your adventures in Middle-Earth with peace of mind, knowing your shared world remains synchronized!
```

In this updated version, I've incorporated the correct `.gitignore` content and made some improvements to ensure clarity, engagement, and a comprehensive understanding of the repository's setup and usage.
