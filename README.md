# swmaptool

Scott's Quick and Dirty Savage Worlds (Adventure Edition) Framework

# Campaign Macros

### General

**Roll Trait**: This asks for a trait name (for display purposes only; 0 displays nothing), die size, and up to three modifiers. It rolls an exploding die of the chosen size and a wild die and displays the higher roll plus the modifiers. If the selected token is not a Wild Card, it does not roll a wild die.

**Autofire**: This asks for a trait name (for display purposes only; Fighting is an option as this macro can also represent Frenzy attacks), rate of fire, die size, and up to three modifiers. It rolls the appropriate number of trait dice and a wild die. If the selected token is not a Wild Card, it does not roll a wild die.

**Set Initiative**: Once you've determined initiative (not always the card you draw, due to edges), select a token and enter its card's value and suit; it will be added to initiative with a sort-friendly initiative value. If the Joker box is checked, the selected value and suit are discarded.

**Prone/Stand**: Toggle Prone status on selected token(s).

**Shaken**: Acts on selected token(s). If not shaken, sets shaken. If shaken, prompts for a spirit roll (with option to auto-succeed.) Only rolls a wild die for Wild Cards. If the roll is a success, removes Shaken status.

**Wounds**: Wound tracking. Applies # of wounds to target; for healing enter a negative number. Automatically tracks wounds and sets statuses appropriately.

**Elevation**: Set token elevation (0 clears the property.)

**OTT** (**O**ff **t**he **T**able): Toggles a big gray **X** over the selected token(s), an extra-visible indicator that something is out of the fight but you don't want to remove the token.

### Tracking

**Bennies**: These macros reset a token's available bennies (2 for NPC Wild Cards, 3 for PC Wild Cards,) spend a benny, or (GM only) adds one benny.

**Wounds**: This macro adds or removes wounds to a token and sets appropriate states. Enter a negative number for healing.

**Fatigue**: This macro adds or removes fatigue from a token and sets appropriate statuses. Multiple Exhausted statuses do not stack; the fatigue offensive power modifier cannot Incapacitate.

### Type

These macros change the selected token(s) to Extras or Wild Cards.

# Campaign Properties

**Status Icons**: These are from RPTroll's framework and can be set manually; macros to set them more quickly will be added later. I've added an icon for "Incapacitated through fatigue"

**Statsheet**: The Parry, DisplayToughness, DisplayPace, and Bennies properties are displayed on the statsheet to the token owner; the Elevation property is shown to all.

**Token Properties**: There are four types -- "Basic" is unchanged from the maptool default, "Deck" is used for card decks, "WildCard" is for Wild Cards, and "Extra" is for Extras. Wild Card and Extra token types include a number of values that can be used for deriving Parry and Toughness and for tracking Wounds, Fatigue, and Bennies.

# Other

## Decks

The "deck" token represents a card deck. Each copy of a deck token tracks its own state (card order and next card position) separately, so you can have as many different decks as you want named whatever you want.

Each deck token has three macros, which are mostly self-explanatory -- Shuffle shuffles the card order and resets the next card position to zero, Draw Card draws one card, and Draw X Cards asks you for a number and draws that many cards. If there are not enough cards left to draw, the macro will display an error and not change state.

