# <!-- {docsify-ignore} -->
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

- The editor window occasionally throws these errors:

    ```
    GUI Error: Invalid GUILayout state in BetterRuleTileEditor view. Verify that all layout Begin/End calls match
    UnityEngine.GUIUtility:ProcessEvent (int,intptr,bool&)

    GUI Error: You are pushing more GUIClips than you are popping. Make sure they are balanced.
    UnityEngine.GUIUtility:ProcessEvent (int,intptr,bool&)  
    ```

    This error also doesn't cause any problems. It mostly gets thrown when a window in the editor changes sizes.

- The random sprites option can behave weirdly. Time and cause of this bug is currently unknown.
- Hexagon grid zooming doesn't center around the mouse cursor properly.
- Sprite drawer cannot be moved