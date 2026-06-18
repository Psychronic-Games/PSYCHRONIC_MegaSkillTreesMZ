# PSYCHRONIC_MegaSkillTreesMZ

**RPG Maker MZ Plugin**

Complete Skill Tree System with Visual Builder

## What It Does

MEGA SKILL TREES MZ - Complete Skill Tree System.

## Plugin File

- `PSYCHRONIC_MegaSkillTreesMZ.js`
- Version: `1.0`
- Target: RPG Maker MZ
- Author: Psychronic
- URL: https://psychronic.itch.io

## Plugin Commands

- `assignTreeToActor`
- `removeTreeFromActor`
- `grantKnowledge`
- `resetSkillTree`
- `openSkillTreeScene`
- `openSkillTreeBuilder`

## Parameter Summary

- builderMode: Enable tree builder interface (only for development/testing)
- autoOpenBuilder: Automatically open builder in browser when game starts
- openBuilderInSystemBrowser: Force builder to open in system browser instead of NW.js window (fixes Linux click offset)
- useExpAsKnowledge: Use actor's total EXP instead of a variable for knowledge points
- expDisplayName: Custom name for EXP when using EXP mode (e.g., "Skill Points", "Training XP")
- knowledgeVariableId: Variable that stores knowledge points (ignored if Use EXP is enabled)
- knowledgeDisplayName: Custom name for knowledge variable mode (e.g., "Skill Points", "Ability Points")
- showLevel: Show actor level in the character info bar
- knowledgeIconIndex: Icon to display next to knowledge cost on nodes (0 = no icon)
- goldIconIndex: Icon to display next to gold cost on nodes (0 = no icon)
- menuCommandName: Name shown in the main menu
- menuCommandShow: Show "Learn Skills" command in main menu
- classColorIndex: Message color code for class name (0-31, use \c[x] colors)
- subclassColorIndex: Message color code for subclass name (0-31, use \c[x] colors)
- skillTrees: Define all available skill trees
- classBasedTrees: Automatically assign trees to actors based on their class
- id: Unique ID for this skill tree
- name: Display name of the skill tree
- iconIndex: Icon to display for this tree
- nodes: All nodes in this skill tree
- id: Unique ID within this tree
- skillId: The skill learned from this node
- x: X coordinate in the tree (pixels)
- y: Y coordinate in the tree (pixels)
- knowledgeCost: Knowledge points required to learn
- Additional parameters are documented in the plugin header/help text.

## Installation

1. Download `PSYCHRONIC_MegaSkillTreesMZ.js`.
2. Place it in your RPG Maker MZ project's `js/plugins/` folder.
3. Enable it from the RPG Maker Plugin Manager.
4. Configure any plugin parameters or commands listed below.

## Full Plugin Help

### MEGA SKILL TREES MZ - Complete Skill Tree System

This plugin provides a complete skill tree system with:
- Visual node-based skill trees
- Knowledge point system for learning skills
- Tree builder interface for easy creation
- Multiple trees per character
- Prerequisites and skill connections

### How to Use

1. Set the Knowledge Variable ID in plugin parameters
2. Create skill trees using the builder (enable Builder Mode)
3. Assign trees to actors using plugin commands
4. Grant knowledge points to players
5. Players can access "Learn Skills" from the menu

### Tree Builder (Development Mode)

When Builder Mode is enabled:
- Press Shift+PageUp to open the builder from menu or skill tree scene
- OR use the plugin command "Open Skill Tree Builder"
- Click to place skill nodes
- Use TAB to switch between modes (Select/Add/Connect)
- Arrow keys to move selected nodes
- Press PageDown to export tree data to console

### Terms of Use
Free for commercial and non-commercial use.

## Source

This standalone repository is generated from the latest PSYCHRONIC plugin source in the RPG Reactor Complex template.

## License

MIT. See `LICENSE`.
