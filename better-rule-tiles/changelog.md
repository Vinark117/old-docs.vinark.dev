# <!-- {docsify-ignore} -->

# Version 1.0.0

Initial release

# Version 1.0.1

- Added support for differently sliced isometric tiles, previously it only supported square sliced sprites.
- Updated package dependencies to reflect the minimum supported versions of packages and unity version.
- The tool now supports Unity 2020

# Report bugs

To report a bug head to [this page](https://itch.io/t/2381185/bug-reports). Please try to not report bugs that have been already reported, to keep the discussion board more organized.

# Known issues

- Editor window throws this error:

    ```
    Resolve of invalid GC handle. The handle is from a previous domain. The resolve operation is skipped.
    UnityEngine.GUILayout:Window (int,UnityEngine.Rect,UnityEngine.GUI/WindowFunction,UnityEngine.GUIContent,UnityEngine.GUILayoutOption[])
    VinToolsEditor.BetterRuleTiles.GUIWindow:Show (int,UnityEngine.Rect) (at Assets/BetterRuleTiles/Editor/EditorSubClasses/GUIWindow.cs:92)
    VinToolsEditor.BetterRuleTiles.BetterRuleTileEditor:DisplayWindows () (at Assets/BetterRuleTiles/Editor/CustomEditor/BetterRuleTileEditor.cs:502)
    VinToolsEditor.BetterRuleTiles.BetterRuleTileEditor:OnGUI () (at Assets/BetterRuleTiles/Editor/CustomEditor/BetterRuleTileEditor.cs:214)
    UnityEngine.GUIUtility:ProcessEvent (int,intptr,bool&)
    ```

    This error does not cause any problems, but unfortunately I wasn't able to find and remove the cause of it.