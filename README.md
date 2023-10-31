# Return to Moria Shared Save Repository

Hail, Fellow Adventurers of Middle-Earth! Welcome to the hallowed grounds of our shared repository, where the essence of our collective journey through the mystic lands of Moria is chronicled and safeguarded.

## Table of Contents

- [Preparing Thy Machine for the Shared Chronicle](#preparing-thy-machine-for-the-shared-chronicle)
- [The Path to the Repository](#the-path-to-the-repository)
- [The Lineage of Branches](#the-lineage-of-branches)
- [The Scrolls of Exclusion](#the-scrolls-of-exclusion)
- [The Council of Contribution](#the-council-of-contribution)
- [Summoning Aid](#summoning-aid)
- [Tales of Yore (FAQs)](#tales-of-yore-faqs)

## Preparing Thy Machine for the Shared Chronicle

Before venturing forth, thou must disable the cloud save feature within the Epic Games launcher, for it meddles with the essence of our shared lore. Be forewarned, this act shall disable cloud saves for all thy games, not merely Return to Moria.

1. Launch the Epic Games launcher and navigate to the `Settings` menu.
2. Scroll down to the `Preferences` and isable the `Enable Cloud Saves` checkbox.

With the cloud's fleeting whispers silenced, thou art now ready to partake in the shared tale of Return to Moria.

## The Scrolls of Exclusion

In the ancient `.gitignore` scroll, runes are inscribed to shroud all but the chosen chronicle from the gaze of Git. Only the file `MW_CA0D1BEC4DB885C03B96F89B3AA5D751.sav` is granted passage through the veil of ignorance to partake in the grand tale of our fellowship.

```plaintext
# Enshroud all files in shadows
*

# But let this chosen chronicle bask in the light
!MW_CA0D1BEC4DB885C03B96F89B3AA5D751.sav


## The Path to the Repository

The sacred repository resides within the heart of your machine, at the following path, waiting to be summoned:

```plaintext
C:\Users\[USERNAMEHERE]\AppData\Local\Moria\Saved\SaveGames
```

Replace `[USERNAMEHERE]` with thy name, O keeper of worlds.

## The Lineage of Branches

The `main` branch, noble and true, holds the latest tale of our adventures in its heart. As the chosen host, thou shalt heed the ancient rites before drawing from its wisdom:

1. Before summoning the essence of our shared journey from the repository, thou must ensure the `SaveGames` chamber is bereft of previous chronicles. Move thy local files to a safe haven:

```bash
# Create a haven for thy current tales
mkdir -p ~/MoriaBackup
mv C:\Users\[USERNAMEHERE]\AppData\Local\Moria\Saved\SaveGames\* ~/MoriaBackup
```

2. Now, navigate to the `SaveGames` chamber and summon the shared lore from the abyss of the repository:

```bash
# Venture into the SaveGames chamber
cd C:\Users\[USERNAMEHERE]\AppData\Local\Moria\Saved\SaveGames

# Ere the gathering:
git clone https://github.com/Syferus/ReturnToMoriaSaves.git .
```

3. Once the shared lore is summoned, thou may restore thy personal chronicles to the `SaveGames` chamber:

```bash
# Restore thy personal tales
mv ~/MoriaBackup/* C:\Users\[USERNAMEHERE]\AppData\Local\Moria\Saved\SaveGames
```

4. Following the gathering's end, inscribe the new tales and share them with the fellowship:

```bash
# Following the gathering's end:
git add .
git commit -m "Tales of our journey on [DATE]"
git push origin main
```

Replace `[USERNAMEHERE]` with thy name, O keeper of worlds, and `[DATE]` with the day of our fellowship's assembly.

May the clear path and shared lore guide thee and thy fellowship through the enchanting halls of Moria!

## The Scrolls of Exclusion

In the ancient `.gitignore` scroll, runes are inscribed to shroud all but the chosen chronicle from the gaze of Git. Only the file `MW_CA0D1BEC4DB885C03B96F89B3AA5D751.sav` is granted passage through the veil of ignorance to partake in the grand tale of our fellowship.

```plaintext
# Enshroud all files in shadows
*

# But let this chosen chronicle bask in the light
!MW_CA0D1BEC4DB885C03B96F89B3AA5D751.sav
```

## The Council of Contribution

We welcome the shared wisdom of all members of our fellowship. Share thy thoughts through issues or pull requests, and together we shall build a tome of knowledge.

## Summoning Aid

Should thou find thyself ensnared in doubts or the dark arts of Git, fear not! Contact the wise keeper of this repository or invoke aid by raising an issue herein.

## Tales of Yore (FAQs)

Unveil the lore and answers to ancient queries that may guide thee on thy quest.

- **Q: How shall I safeguard my personal chronicles?**
- **A:** ’Tis the duty of every soul to guard their own tale. Back up thy data in the realms of your own machine.

- **Q: What if the spirits of Sync play foul tricks?**
- **A:** Raise thy voice through an issue in this repository, and together we shall banish the foul spirits back into the void.

May the Valar guide thee on your quests within the depths of Moria, as the shared lore of our fellowship continues to echo through the annals of this repository!
