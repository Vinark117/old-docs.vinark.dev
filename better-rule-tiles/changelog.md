# <!-- {docsify-ignore} -->

# Version 0.1.0

Initial release

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