# New Level Up Screen

**Advanced learning of secondary skills with full ACM compatibility**

## 📖 Description

New Level Up Screen is a comprehensive Heroes 3 plugin that completely overhauls the level-up experience. Instead of being limited to just two randomly selected secondary skills, this mod allows you to choose from **all available secondary skills** during level-up, giving you full control over your hero's development.

### ✨ Key Features

- **🎯 Choose Any Available Skill**: Select from all secondary skills your hero can learn, not just two random options
- **🔗 Full Mod Integration**: 
  - Seamlessly works with Advanced Classes Mod (ACM)
  - Complete compatibility with More_SS_Levels plugin
- **🌍 Multi-Language Support**: Uses in-game text and mod translations for maximum language compatibility
- **⚙️ Configurable**: Customize skill availability through config settings or use More_SS_Levels config for extended limits
- **📊 Enhanced UI**: Improved dialogs with better visual feedback and information
- **🎮 Intuitive Controls**: 
  - Single-click to preview skills
  - Double-click to instantly select and confirm
  - Right-click for detailed skill information
- **🏆 Artifact Integration**: Primary skill tooltips show base values and artifact bonuses

## 🚀 Installation

1. Extract the mod to your Heroes 3 ERA `Mods` folder
2. Ensure Advanced Classes Mod is installed if you want ACM compatibility
3. Launch the game and enjoy enhanced level-ups!

## ⚙️ Configuration

Edit `Data\NewLevelUpScreen.cfg`:

```ini
[NewLevelUpScreenSettings]
; Controls whether to use original game probability restrictions for secondary skills
; 0 = Use original game probabilities - Only skills with >0% chance can be learned (Default)
; 1 = Remove probability restrictions - All secondary skills can be learned regardless of hero class
; Note: Setting this to 1 allows any hero to learn any secondary skill, ignoring class restrictions
RemoveZeroProbability=1

; Maximum number of secondary skills each hero can learn
; Valid range: 1-28
; Default: 8 (vanilla Heroes 3 limit)
; Note: More SS Levels mod setting takes precedence if active
SecondarySkillLimit=12
```

## 🔧 Compatibility

### ✅ Fully Compatible
- **Advanced Classes Mod (ACM)**: Complete integration with dynamic behavior based on ACM settings
- **More_SS_Levels Plugin**: Full support for extended secondary skill systems (requires latest version)
- **ERA 3.x Framework**: Built as a native ERA plugin for maximum stability
- **Secondary Skill Limit Systems**: 
  - Built-in configurable limits
  - More_SS_Levels extended limits
  - Legacy mods (10SSkills, No Secondary Skills Limit, etc.)
- **Resolution Mods**: Safe dialog positioning works with any screen resolution
- **Language Packs**: Uses game's native text system for full localization support

### ⚠️ Potential Conflicts
- **Other Level-Up Mods**: May conflict with mods that also modify the level-up process
- **Skill System Overhauls**: Unknown compatibility with major skill system changes

### 🔄 ACM Behavior Modes
- **Standard ACM Mode**: Respects ACM skill dependencies and point requirements
- **Berserker Mode**: Adapts when ACM's "No Skill Dependencies" option is enabled
- **Vanilla Mode**: Falls back to standard Heroes 3 behavior when ACM is not active

## 📋 Changelog

### Version 3.1 (Current)
- **🔗 More SS Levels Integration**: Full compatibility with the More_SS_Levels plugin (requires latest version)
- **⚙️ Independent Config System**: No longer relies on external plugins/patches/ERM for secondary skill limits - uses built-in config options
- **🔧 Simplified Setup**: If using More_SS_Levels, edit its config for skill limits instead of NewLevelUpScreen config
- **🐛 Minor Fixes**: Various stability improvements and code optimizations

### Version 3.0
- **🔄 Complete Rewrite**: Rebuilt the entire plugin from scratch for better maintainability
- **🔧 Improved Hooks**: Changed to more compatible hook points to reduce conflicts with other mods
- **🛠️ Fixed Crashes**: Resolved critical dialog closing crashes and memory management issues
- **🎨 Enhanced UI**: 
  - Better visual feedback for skill availability
  - Improved skill level indicators
  - Smoother dialog animations
- **🖱️ Double-Click Support**: Added double-click to instantly select and confirm skills
- **📐 Bounds Checking**: Dialogs now properly stay within screen bounds on all resolutions
- **🌐 Improved Text System**: 
  - Better skill name and description display
  - Fixed text duplication issues
  - Proper skill level text formatting
- **⚡ Performance Optimizations**: Faster dialog creation and rendering
- **🏆 Artifact Display**: Primary skill info now shows base values vs. total with artifacts

### Version 2.0
- **🤝 Full ACM Integration**: Complete compatibility with Advanced Classes Mod
- **🗣️ Multi-Language Support**: Uses in-game text and ACM translations for broad language support
- **🔌 Plugin Architecture**: Converted from pure ERM to native plugin with ERM components for ACM
- **⚙️ Configuration System**: Added config file with RemoveZeroProbability setting
- **📊 Skill Limit Support**: Proper integration with custom secondary skill limit systems
- **🎯 Enhanced Primary Skills**: Right-click information dialogs with detailed statistics

### Resolved Issues
- **✅ Dialog Crashes**: Fixed in version 3.0
- **✅ Memory Leaks**: Resolved with better resource management
- **✅ Text Display Problems**: Fixed skill name and description rendering
- **✅ Resolution Conflicts**: Added proper bounds checking for all screen sizes