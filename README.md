<div align="center">
  <a href="https://github.com/scribe-org/Scribe-iOS"><img src="https://github.com/scribe-org/Scribe-iOS/blob/main/Resources/Scribe-iOS_logo_transparent.png" width=612 height=164></a>
</div>

---

<!--
[![license](https://img.shields.io/github/license/scribe-org/Scribe-iOS.svg)](https://github.com/scribe-org/Scribe-iOS/blob/main/LICENSE.txt)
-->

[![coc](https://img.shields.io/badge/coc-Contributor%20Covenant-ff69b4.svg)](https://github.com/scribe-org/Scribe-iOS/blob/main/.github/CODE_OF_CONDUCT.md)

[![Available on the App Store](http://cl.ly/WouG/Download_on_the_App_Store_Badge_US-UK_135x40.svg)](https://www.apple.com/app-store/)

### Scribe language keyboards for iOS

**Scribe-iOS** is a pack of iOS and iPadOS power user keyboards for language learners. Features include verb conjugation and gender based annotation of nouns that give users the tools needed to communicate with confidence. Being fully open-source, Scribe prioritizes user privacy and doesn't ask for access to any user data. German and Spanish are currently the only supported languages, but the Scribe team has interest in creating keyboards for all languages of interest.

# **Contents**<a id="contents"></a>

- [Setup](#setup)
- [Features](#features)
- [To-Do](#to-do)

# Setup [`↩`](#contents) <a id="setup"></a>

Users access Scribe language keyboards through the following:

- Download Scribe from the [App Store](https://www.apple.com/app-store/)
- Settings -> General -> Keyboard -> Keyboards -> Add New Keyboard
- Select from the available Scribe keyboards
- When typing press 🌐 to select keyboards

# Features [`↩`](#contents) <a id="features"></a>

## Grammar Queries

Scribe allows users to query words based on grammar rules. This is done via the `Scribe key` at the top left of any Scribe keyboard. Pressing this key gives the user two new selectable options: `Conjugate` and `Plural`. In the case of `Conjugate`, a user types in a verb, presses the `↵` key, and then is presented with the grammar charts for the given verb instead of the keyboard. Pressing an example in the charts would then insert the chosen conjugation into the text field. In the case of `Plural`, a user types a noun, presses return, and then the plural would be inserted into the text field. An extra space is inserted after the queried word so that this feature functions similar to auto-suggestions.

## Noun-Gender Annotation

Scribe annotates nouns according to the following conventions:

- Feminine nouns are colored red 🟥 and marked with (F)
- Masculine nouns are colored blue 🟦 and marked with (M)
- Neutral nouns are colored green 🟩 and marked with (N)
- Plural nouns are colored orange 🟧 and marked with (PL)
- Multi gendered nouns are multicolored and marked with all their genders

<!--
Genders are displayed once a user has typed a noun and pressed space or while a noun is selected.
-->

## iOS and iPadOS System Keyboard Functionality

The goal is that Scribe keyboards have all the functionality of system keyboards.

<details><summary><strong>Currently implemented features</strong></summary>
<p>

- iPhone and iPad support (WIP)
- Dynamic layouts for cross-device performance
- Portrait and landscape views (WIP)
- Auto-capitalization
- The double space period shortcut
- Typing `'` returns to the alphabetic keyboard
- Dark mode compatibility (WIP)
- Hold-to-select characters (WIP)

</p>
</details>

# To-Do [`↩`](#contents) <a id="to-do"></a>

Please see the [contribution guidelines](https://github.com/scribe-org/Scribe-iOS/blob/main/.github/CONTRIBUTING.md) if you are interested in contributing to this project. Work that is in progress or could be implemented includes:

- Allowing for grammar queries from json files

- Expanding Scribe's support for current languages by adding to the [grammar files](https://github.com/scribe-org/Scribe-iOS)

  - Nouns should have their gender and plural

  - Verbs should have all conjugations

  - Pull requests are more than welcome!

- Adding support for more languages to Scribe-iOS [(see issues)](https://github.com/scribe-org/Scribe-iOS/issues)

- Selecting a noun would display its gender in the preview bar [(see issue)]()

- Localizing the Scribe app across various languages and regions [(see issues)](https://github.com/scribe-org/Scribe-iOS/issues)

- Allowing words to be colored within preview texts such that the user will consistently see their gender [(see issue)]()

- Exploring the possibility of translations [(see issue)]()

  - This would add another option to the `Scribe key` where entering a word in the preview bar would bring up a selectable list of translations over the keyboard

  - The base functionality would translate from the system language into the language of the keyboard, with the ability to choose a language from which translations would be made being ideal

- Moving grammar files to a new repository in [scribe-org](https://github.com/scribe-org) and accessing them remotely to allow Android and extension access [(see issue)]()

  - This would likely best be implemented via a Python package that allows users to access data within JSON files stored in the package

  - The creation of a repository with grammar rules for Scribe languages would be a valuable resource for Scribe and the open-source community

- Converting Scribe keyboards into downloadable packs within the app [(see issue)]()

  - This would help keep the app size to a minimum

- Make the shift key character change color after being pressed [(see issue)]()

  - Note: we want ⇧ to switch to `⬆` and ⇪ to also be filled in

- Make the space bar read the name of the keyboard when it's switched to [(see issue)]()
