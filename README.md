# Singleton
$hHandle = WinGetHandle(@ScriptDir)         ControlSetText($hHandle, '', ControlGetHandle($hHandle, '', 'Edit1'), @AutoItPID)     Else         If BitAND($iFlag, 1) Then             Return Number(ControlGetText($hHandle, '', ControlGetHandle($hHandle, '', 'Edit1')))         Else             Exit -1         EndIf     EndIf     Return 0 EndFunc   ;==>_SingletonFolderInstance
