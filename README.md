![poster](./assets/poster.png)

Velocity is a modern, **kinetic** theme for Obsidian. Bold and _opinionated_, the theme appears subtle on the surface, but dares to reimagine what the Obsidian user interface experience can be.   

Velocity draws heavy inspiration from MacOS design principles and contemporary web aesthetics. It evokes a clean, yet playfully mechanical, almost tactile kind of modernity. The theme is also inspired by the sleek user interfaces of various mid-to-late-2000s **racing games** - hence its name. 

Velocity is close to the end of its ``alpha`` development and is fast approaching ``beta`` readiness. Therefore, while it is _very_ polished in many areas, it may still be broken or incomplete in others. 

## Table of Contents

- About
- [Installation](#Installation)
- [Images](#Images)
- [FAQ](#FAQ)
- [Roadmap](#Roadmap)
- [Background](#Background)
- [Credits](#Credits)

## Installation
Velocity is not officially released on the Obsidian store. Currently, the easiest method to install the theme is by using the **BRAT** plugin in Obsidian. Simply paste the link of the main branch of the repository in the BRAT plugin's settings. BRAT automatically handles changes made upstream by checking for any new changes in the repo upon launching Obsidian, ensuring that you always have the most up-to-date version of Velocity.

Alternatively, you can opt to download the files manually. You will need the ``theme.css`` and ''manifest.json`` files. Create a folder named "Velocity" inside the Obsidian themes folder, located at ``your-vault/.obsidian/themes``, and place the files inside. The theme should show up in the Appearance tab the next time you open the vault.

## Images 

#### Editor
![Headings](./assets/headings.png)
![Callouts](./assets/callouts.png)
![Multiple tabs](./assets/multiple-tabs.png)

#### Interface
![Command Palette](./assets/command-palette.png)
![Bookmark](./assets/bookmark.png)
![Settings](./assets/settings.png)
![Graph Controls](./assets/graph-controls.png)

## FAQ
- **Do I have to buy Velocity?**
  - No. The theme is free, as it should be.
- **What kind of user is this theme designed for?**
  - Velocity is designed for creatives, thinkers and note-takers of all kinds, those who love good looking apps with smooth interactions, and users who want their vault to look premium and polished. It will please users looking for a balanced degree of customization features, without overwhelming with too many options to tweak. Fans of Swiss Design, early 2010s Apple graphics design, and 2000s racing games will feel right at home.
  - Velocity is not designed for absolute minimalists. It is not designed for absolute maximalists, either. It is probably not ideal for power users seeking terminal UI aesthetics, nor is it suitable for those who want something fuzzy and warm. It is not designed for people who wish to have absolute, total control over customization. Lastly, it is not a theme for those afraid to try something bold, innovative and new.
- **How can I customize the theme?**
  - Download the Style Settings plugin from within the Obsidian app's plugin store. The plugin is free as are most plugins, and the settings for Velocity should appear automatically so long as you have the theme enabled.
- **How long have you been working on this?**
  - Velocity has been in ``alpha`` for approximately 8 months as of July 2025; development started in late November last year as a pure passion project. 8 months worth of scope creep and constant improvement has led the project to where it is now, but I can assure you that it won't be in ``alpha`` for much longer.
- **Why should I choose Velocity? What makes it different from other themes?**
  - If there is ONE reason to at least _try_ Velocity, it is because nearly no other theme is crafted with as much attention to detail in the user interface department. Countless hours have been spent making sure interactions, spacing, color balance and texture feel _just right_. In simple terms, Velocity is designed to make you feel as if you were using a premium, paid app - to make you forget even for a moment that you're in Obsidian.
  - Markdown has received much love, too, even if it is not always the main focus. Velocity offers typographic alignment tweaks and features that might please some typography enthusiasts. It is the _only_ theme which accounts for heading indent misalignment with larger headings. It is also perhaps best-in-class when it comes to callout manipulation - you can put just about anything inside of them, such as headings, code, Dataview queries and more, and it _will look good_. 
  - And if all of this fails to convince you, maybe just the novelty of a theme designed over the course of nearly a whole year, with an inspiration as idiosyncratic as _racing game user interfaces_, might convince you.
- **Will you add feature X/Y/Z to Velocity?**
  - It depends. Certain features you may be looking for might already be present in the theme. Others which are missing may be added or rejected based on whether the feature is aligned with Velocity's overall philosophy, or whether the feature is better off as some snippet due to complexity/feature creep. In any case, please make requests for features in the **Issues** page or in the Obsidian **Discord** thread for Velocity.
- **Will this theme work with plugin X/Y/Z?**
  - As an opinionated UI-centric theme, Velocity may interfere with the styling of some plugins' settings or modals in a way that is not intended or aesthetic. This is a necessary and inevitable tradeoff when designing a theme which alters the default UI to such an extent. Nevertheless, in my own testing, most plugins work just fine with Velocity. The worst you'll experience in most cases is some minor menu jank, but functionality of plugins should be **totally unaffected.**
- **Why does it look so much like theme X/Y/Z?**
  - Velocity has been created with multiple inspirations in mind, including various themes I used for my own vaults before deciding to make my own. The most obvious parallels are to the wonderful **[Cupertino](https://github.com/aaaaalexis/obsidian-cupertino)** theme, which is a result of that theme's innovations and approaches inspiring an entire generation of new themers. However, Velocity differs from Cupertino in many ways once you look past the surface level. At their core, the two themes are fundamentally different in approach and philosophy.
  - The keen-eyed user or fellow theme developer may notice some paralles with the beautifully tactile **[Primary](https://github.com/primary-theme/obsidian)** by Cecilia May. This is because I have taken much inspiration from her exacting attention to detail and focus on tactile responsiveness in UI interactions. 
  - I have detailed the full list of works I have drawn inspiration or borrowed code from in the Credits section of the README. **Any other resemblances are thus purely coincidental.** In any case, I do not intend to merely copy or imitate the work of a fellow theme dev. 
- **Why does the theme look different from before?**
  - If you have been around since the earlier alphas (up until the ``0.6.x`` versions) then you may notice the theme is no longer retro or skeuomorphic. This is because I quickly realized that the theme would never appeal to a larger audience and my specific design ideas and obsessions would forever remain obscure and niche. 
  - While the ``1.0.0`` revamp to a more modern, minimalist style was informed by outside pressures, this does not mean that Velocity has lost its character or 'soul'. I have made sure that key design elements and quirks are carried over from the older versions. Several users have testified that they enjoy the current versions _even more_ than the old ones.
  
## Background

Under construction

## Roadmap

Beta is estimated to be ready in **2-3 months**, by version ``1.2`` or ``1.3``. 
Expect a full release before or during Obsidian October.

## Credits

#### Themes:

**Sanctum** - the main theme I used in the past and a major influence on Velocity's typography.

**Border, Primary & Mado** - major influences and sources of code for earlier versions of Velocity. Primary in particular informs this theme's approach to never leave any detail untouched.

**Cupertino & Composer** - modern themes which influenced the current iteration of Velocity. 

**Willemstad** - a source of inspiration for the modified community themes page in both old and new versions of Velocity.

**Micro Mike** - its "mini-mode" is the basis for Velocity's Auto-hide feature.

### People:

Under construction
