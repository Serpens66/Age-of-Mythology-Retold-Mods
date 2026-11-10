# XS and console reference comparison

Retail is the Doxygen archive shipped with the installed 19.17020 snapshot.
The local `doxygen_old_aber_mehr` snapshot has no verified build identifier.
These are documentation differences. An old declaration is a lead for a test in
the appropriate execution context. An absent declaration does not establish removal
from the runtime. Console, UI and XS contexts require separate verification.

Compared the Functions and Variables summary tables on Doxygen source pages. Keys
are symbol kind, name and normalized declaration. A changed declaration can reflect
a parameter rename or formatting as well as a changed type or argument list.

| Source page | Retail functions / variables | Older functions / variables |
| --- | ---: | ---: |
| `aconsolefuncs_8cpp.html` | 0 / 0 | 59 / 0 |
| `aifuncs_8cpp.html` | 215 / 0 | 212 / 0 |
| `aiplans_8cpp.html` | 0 / 193 | 0 / 192 |
| `consolefuncs_8cpp.html` | 0 / 0 | 168 / 0 |
| `consolefuncsmp_8cpp.html` | 0 / 0 | 9 / 0 |
| `consolefuncstech_8cpp.html` | 0 / 0 | 22 / 0 |
| `consolefuncstestharness_8cpp.html` | 0 / 0 | 0 / 0 |
| `consolefuncsui_8cpp.html` | 0 / 0 | 368 / 0 |
| `kbarmyfuncs_8cpp.html` | 23 / 0 | 23 / 0 |
| `kbfuncs_8cpp.html` | 423 / 0 | 360 / 0 |
| `kbprogressionfuncs_8cpp.html` | 6 / 0 | 6 / 0 |
| `kbtechtreefuncs_8cpp.html` | 32 / 0 | 16 / 0 |
| `randommapfuncs_8cpp.html` | 502 / 0 | 404 / 0 |
| `triggerfuncs_8cpp.html` | 410 / 0 | 313 / 0 |
| `triggerfuncs__mainthread_8cpp.html` | 105 / 0 | 81 / 0 |
| `xsfuncs_8cpp.html` | 90 / 0 | 86 / 0 |

Retail unique declarations: 1,806 functions, 193 variables.
Older unique declarations: 2,127 functions, 192 variables.
Shared identical declarations: 1,242.
Shared names with a declaration difference: 359.

## Older-only symbols

<details><summary>aconsolefuncs_8cpp.html (59 declarations)</summary>

- `bool doMPSetup (bool useESO, bool useRelicLink)`
- `void abortCinematic ()`
- `void activatePhotoScreen ()`
- `void chat (string text, int playernum)`
- `void doSPDeathMatchSetup ()`
- `void doSPSupremacySetup ()`
- `void dropToMainMenu ()`
- `void enterRecordGameMode (string ansiName)`
- `void exitMPSetupSubScreen ()`
- `void hideGameMenu (bool playSound)`
- `void holdToAbortCinematic (int keystate)`
- `void leaveGame (int fromMode, int reason)`
- `void minimapRotateMode (int mode)`
- `void minimapZoom (float delta)`
- `void minimapZoomDelta (float delta)`
- `void openPhotoScreen ()`
- `void playerResign ()`
- `void postGame ()`
- `void postGamePlayAgain ()`
- `void resetCameraPhotoScreen ()`
- `void restartCurrentGame ()`
- `void restartCurrentGameWithSeed (int seed)`
- `void retellCurrentGame ()`
- `void scoreUpdate ()`
- `void sendPromptType (int sendingPlayer, int promptType)`
- `void setIgnoreAsserts (bool ignore)`
- `void setRlinkMpMode (int rlinkMpMode)`
- `void setSunPosition (float inclination, float rotation, bool relative)`
- `void showCampaignDialog (string nextCampaign, string string)`
- `void showGameFromPostGame ()`
- `void showGameMenu ()`
- `void startBlankGame (int numberPlayers)`
- `void startRandomGame (bool editorMode)`
- `void startRandomGame2 (string filename, int numberPlayers, int teamCount, int seed, int size)`
- `void startRandomGameAgeAndMapCode (int startAge, bool nomad, string mapcode)`
- `void startRandomGameMapCode (string mapcode)`
- `void startRandomGameMapCodeAI (string mapcode, bool enableAI)`
- `void sunDecreaseInclination (int keyState)`
- `void sunDecreaseRotation (int keyState)`
- `void sunIncreaseInclination (int keyState)`
- `void sunIncreaseRotation (int keyState)`
- `void toggleDebugTime ()`
- `void toggleGameMenu ()`
- `void toggleScore ()`
- `void toggleTime ()`
- `void toggleUIPhotoScreen ()`
- `void uiNewScenario ()`
- `void uiRefreshEditorMenu ()`
- `void uiSpecialPowerAtPointer ()`
- `void uiToggleDiplomacyDialog ()`
- `void uiToggleGame ()`
- `void uiZoomToMinimapEvent ()`
- `void uiZoomToMinimapEvent2 ()`
- `void windowsStore_BlockRatingPrompt ()`
- `void windowsStore_HideRatingPrompt ()`
- `void windowsStore_ShowRatingPrompt ()`
- `void windowsStore_TryShowRatingPrompt ()`
- `void windowStore_LaunchRatingURI ()`
- `void XBLSignInOut ()`

</details>

<details><summary>aifuncs_8cpp.html (19 declarations)</summary>

- `float aiGetMinimumFutureNeedsCostPerResource (int escrowID, int planPriority, int resourceID)`
- `float aiGetResourceBreakdownPercentage (int resourceID, int resourceSubTypeID, int baseID)`
- `float aiGetResourceGathererPercentage (int resourceID, int rgpIndex)`
- `float aiGetResourceGathererPercentageWeight (int rgpIndex)`
- `float aiPlanGetUnitCost (int planID, bool considerHitPoints)`
- `float[] aiGetMinimumFutureNeedsCost (int escrowID, int planPriority)`
- `int aiCommsGetStatementPlayerID (int recordID)`
- `int aiCommsGetStatementPromptType (int recordID)`
- `int aiGetScore (int playerID)`
- `int aiPlanGetUnitStance (int planID)`
- `vector aiCommsGetStatementPosition (int recordID)`
- `void aiNormalizeResourceGathererPercentages (int rgpIndex)`
- `void aiNormalizeResourceGathererPercentageWeights ()`
- `void aiPlanSetUnitStance (int planID, int stance)`
- `void aiSetEscrowsDisabled (bool v)`
- `void aiSetResourceGathererPercentage (int resourceID, float percentage, bool normalize, int rgpIndex)`
- `void aiSetResourceGathererPercentageWeight (int rgpIndex, float weight)`
- `void aiUnitSetEconomicRallyPoint (int unitID, vector location)`
- `void aiUnitSetMilitaryRallyPoint (int unitID, vector location)`

</details>

<details><summary>aiplans_8cpp.html (27 declarations)</summary>

- `const int cAttackPlanAllowMoreUnitsDuringAttack = 19`
- `const int cAttackPlanAttackModeMaxChaseDistance = 12`
- `const int cAttackPlanAttackRoutePattern = 2`
- `const int cAttackPlanMovementTypeFlags = 25`
- `const int cAttackPlanRefreshFrequency = 23`
- `const int cAttackPlanRetreatMode = 18`
- `const int cDefendPlanNoTargetTimer = 12`
- `const int cDefendPlanRefreshFrequency = 14`
- `const int cExplorePlanAreaPathWaypoints = 20`
- `const int cFishPlanBreakDownID = 4`
- `const int cFishPlanNoDamageTakenRetreatTimeout = 5`
- `const int cFishPlanStartRetreatTime = 6`
- `const int cTransportPlanBestDangerArea = 14`
- `const int cTransportPlanBestDangerValue = 15`
- `const int cTransportPlanGatherArea = 6`
- `const int cTransportPlanGatherAreaGroup = 4`
- `const int cTransportPlanIgnoreAreaIDs = 13`
- `const int cTransportPlanMaximizeXportMovement = 11`
- `const int cTransportPlanMiddleAreaGroups = 18`
- `const int cTransportPlanPathPlanned = 9`
- `const int cTransportPlanPathType = 8`
- `const int cTransportPlanPersistent = 17`
- `const int cTransportPlanTakeMoreUnits = 19`
- `const int cTransportPlanTargetArea = 7`
- `const int cTransportPlanTargetAreaGroup = 5`
- `const int cTransportPlanTransportTypeID = 1`
- `const int cTransportPlanUnitsMoved = 12`

</details>

<details><summary>consolefuncs_8cpp.html (168 declarations)</summary>

- `void ability (int abilityID, int unitID, bool doWhenNotSelected)`
- `void alignResources ()`
- `void alignSelectedUnits ()`
- `void autoAbility (int abilityID, bool isAutoCasted)`
- `void benchmark ()`
- `void cameraBackward (int keyState)`
- `void cameraDown (int keyState)`
- `void cameraDump ()`
- `void cameraForward (int keyState)`
- `void cameraHome ()`
- `void cameraLeft (int keyState)`
- `void cameraLimit (int arg)`
- `void cameraLocalYawLeft (int keyState)`
- `void cameraLocalYawRight (int keyState)`
- `void cameraMaxZoomSet (float zoom)`
- `void cameraMinZoomSet (float zoom)`
- `void cameraNice ()`
- `void cameraPitchAngle (float angle)`
- `void cameraPitchBackward (int keyState)`
- `void cameraPitchForward (int keyState)`
- `void cameraPitchReset ()`
- `void cameraRight (int keyState)`
- `void cameraRollLeft (int keyState)`
- `void cameraRollRight (int keyState)`
- `void cameraRotate (int arg)`
- `void cameraRotationReset ()`
- `void cameraSetRotationAngle (float degrees)`
- `void cameraStart (int playerID)`
- `void cameraUp (int keyState)`
- `void cameraWorldBackward (int keyState)`
- `void cameraWorldBackwardLeft (int keyState)`
- `void cameraWorldBackwardRight (int keyState)`
- `void cameraWorldForward (int keyState)`
- `void cameraWorldForwardLeft (int keyState)`
- `void cameraWorldForwardRight (int keyState)`
- `void cameraXAxis (float axisValue)`
- `void cameraYawLeft (int keyState)`
- `void cameraYawRight (int keyState)`
- `void cameraYAxis (float axisValue)`
- `void cameraZoomAxis (float axisValue)`
- `void cameraZoomReset ()`
- `void cancelRepairUnit (int unitID)`
- `void cancelTrainReinforcement (int armyID)`
- `void castGodPower (string godPower)`
- `void castGodPowerAtSlot (int slotID)`
- `void commandResearch (int commandID, int unitID)`
- `void config (string token)`
- `void configDef (string name)`
- `void configSet (string name, string value)`
- `void configSetFloat (string name, float value)`
- `void configSetInt (string name, int value)`
- `void configToggle (string name)`
- `void configUndef (string name)`
- `void console ()`
- `void continueToScenario ()`
- `void deleteUnit (int unitID)`
- `void displayType (int val)`
- `void doAbilityInSelected (string protoPowerName)`
- `void doAbilityInType (string protoPowerName, string protoUnitName)`
- `void doCommandInSelected (string commandName)`
- `void doCommandInSelected2 (string commandName)`
- `void echo (string text)`
- `void echoLocalized (int stringID)`
- `void echoNum (int num)`
- `void EconomyVictory ()`
- `void ejectAll (int unitID)`
- `void executeCommandOnButtonPos (int row, int column, bool isSecondaryCommand)`
- `void exit (bool confirmation)`
- `void fov (float newFov)`
- `void gamepadCameraRotate (float axisValue)`
- `void handleCameraBackward (int keyState)`
- `void handleCameraForward (int keyState)`
- `void hideUI ()`
- `void IMEEnable (bool enable)`
- `void imguiconsole ()`
- `void initDefaultHardwareSettings (int hardwareQuality, int windowWidth, int windowHeight, int displayMode)`
- `void kothVictory ()`
- `void leaveBenchmark ()`
- `void loadBackgroundScenario (string scenarioName)`
- `void loadCamera (string filename)`
- `void loadCampaignScenario (string scenarioName)`
- `void loadGame (string fname)`
- `void loadNextCampaignScenario ()`
- `void loadRecentFile (string filename)`
- `void loadScenario (string scenarioName)`
- `void loadTutorial (string tutorialName, int nLoadMode, string loadingScreen, int nTextID)`
- `void loadTutorialWpf (string tutorialName, int nLoadMode, string wpfLoadImage, int nTextID)`
- `void map (string eventName, string context, string command, bool allowInGamepadMode)`
- `void modeEnter (string modeName)`
- `void modeToggleBetweenIfNotMP (string modeName1, string modeName2)`
- `void musicPlaySong (string szName, float fFade)`
- `void musicSetVolume (float fv)`
- `void musicStop ()`
- `void musicToggleBattleMode ()`
- `void obscuredUnitToggle ()`
- `void observingCycleCurrentPlayer ()`
- `void observingToggleFogOfWar ()`
- `void openPrefabsDialog ()`
- `void pause (int val, bool checkForAllowPause)`
- `void pause2 (int val, bool checkForAllowPause)`
- `void playMovie (string fileName)`
- `void relicCapture ()`
- `void renderBaseID (int playerID, int baseID, int state)`
- `void renderForceReset ()`
- `void renderFriendOrFoe (int val)`
- `void renderPlanID (int playerID, int planID, int state)`
- `void renderWindow (int val)`
- `void repairUnit (int unitID)`
- `void res (int xRes, int yRes)`
- `void resetDefaultPlayerColors ()`
- `void resourceMarket (int playerID, string toResourceName, float resourceAmount, string fromResourceName, bool shiftGivesMultiple)`
- `void restart ()`
- `void saveCamera (string filename)`
- `void saveGame (string fname, bool throttleSaves)`
- `void saveScenario (string fname)`
- `void screenshot (int param0)`
- `void setDropDefaultMips (int num)`
- `void setDropTerrainMips (int num)`
- `void setGraphicDetail (int detailLevel)`
- `void setMinimapUnitFilter (int id)`
- `void setShadowBiasMul (float mul)`
- `void setShadowQuality (int level)`
- `void setShadowRotationOp (int rotationOpFlag)`
- `void setShadowSnapping (int snapFlag)`
- `void setSquadMode (string squadModeName)`
- `void setStance (string stanceName)`
- `void setStoryMode ()`
- `void setWorldDifficulty (int v)`
- `void showSPCNote (string title, string text)`
- `void skipNextCampaignScenario ()`
- `void spectateRate (float rate)`
- `void squadMode (int squadModeID)`
- `void squadWheel (float angle, int squadID)`
- `void startCampaign (string filename)`
- `void startMoviePlayback (string filename, int sizing, float fadeIn, float fadeOut)`
- `void stopTrackingAllOfDebugUIState (int debugUIType)`
- `void stopTrackingDebugUIState (int debugUIType, int playerID, int referenceID)`
- `void supaScreenshot (int xRes, bool singleImage)`
- `void toggleShadows ()`
- `void trackAddWaypoint ()`
- `void trackAdvance (float lPosition)`
- `void trackClear ()`
- `void trackCopy ()`
- `void trackEditWaypoint ()`
- `void trackGotoSelectedEvent (int index)`
- `void trackGotoSelectedWaypoint (int index)`
- `void trackInsert ()`
- `void trackPause ()`
- `void trackPlay (float lDuration, int eventID)`
- `void trackRemove ()`
- `void trackRemoveWaypoint ()`
- `void trackSetSelectedWaypoint (int index)`
- `void trackStepBackward ()`
- `void trackStepForward ()`
- `void trackStop ()`
- `void trackToggleShow ()`
- `void trainReinforcement (int armyID)`
- `void uiEnterGameMenuModeIfNotResigned ()`
- `void unitData (int unitID)`
- `void unitDecVariation (int unitID)`
- `void unitIncVariation (int unitID)`
- `void unitReturnToWork ()`
- `void unitSetStance (int stanceID)`
- `void unitSetTactic (string name)`
- `void unitSetVariation (int variation, int unitID)`
- `void unitTownBell ()`
- `void unpauseNoChecks ()`
- `void vsync (int state)`

</details>

<details><summary>consolefuncsmp_8cpp.html (9 declarations)</summary>

- `void invite ()`
- `void inviteCancel (int playerRLinkId)`
- `void inviteExecute ()`
- `void invitePlayer (int playerRLinkId)`
- `void inviteReply (int playerRLinkId, int sessionId, bool accept)`
- `void inviteShowInvitationsExtended ()`
- `void inviteShowInvitationsReceived ()`
- `void inviteShowInviteables ()`
- `void rlAccountCreate (string accountName)`

</details>

<details><summary>consolefuncstech_8cpp.html (22 declarations)</summary>

- `void autoTrainInSelected (string protoName)`
- `void autoTrainInSelectedByID (int protoUnitID)`
- `void cancelAllQueuedInSelected ()`
- `void cancelResearchInSelected (int techID)`
- `void cancelTrainInSelected (int protoID, bool all)`
- `void click ()`
- `void commandResearchInSelected (string cmdName)`
- `void commandTransformInSelected ()`
- `void listTechTree (int playerID)`
- `void preQueueInSelected (string name, bool tech)`
- `void preQueueInSelectedByID (int id, bool tech)`
- `void researchByID (int techID, int unitID, int playerID, bool playClick)`
- `void researchTechInSelected (string techName)`
- `void techDumpMemory ()`
- `void techGetStatus (string name, int playerID)`
- `void techSetCost (string name, string resourceName, int amount, int playerID)`
- `void techSetResearchPoints (string name, int points, int playerID)`
- `void techSetStatus (string name, string status, int playerID)`
- `void tis (string protoName, int count, bool each)`
- `void trainByID (int protoUnitID, int number, int unitID, int playerID)`
- `void trainInSelected (string protoName, int count, bool each)`
- `void trainInSelectedByID (int protoType, int count, bool each)`

</details>

<details><summary>consolefuncsui_8cpp.html (368 declarations)</summary>

- `bool gadgetScrollDown (string gadget)`
- `bool gadgetScrollLeft (string gadget)`
- `bool gadgetScrollRight (string gadget)`
- `bool gadgetScrollUp (string gadget)`
- `void AIDebugGathererToggle ()`
- `void AIDebugInfoRefresh ()`
- `void AIDebugInfoToggle ()`
- `void AIDebugOutputToggle ()`
- `void AIDebugPopToggle ()`
- `void AIDebugShowAreaDangerRatingsToggle ()`
- `void AIDebugShowBasesToggle ()`
- `void AIDebugShowExtendedAreaInformationToggle ()`
- `void AIDebugShowPlansToggle ()`
- `void AIDebugShowPlansToggleAll ()`
- `void AIDebugTimedStatsToggle ()`
- `void AIDebugToggleBPText ()`
- `void closeFlareType (int keystate)`
- `void dirtyMinimap ()`
- `void doTriggerImport (string fn)`
- `void editMode (string modename)`
- `void enterAttackMoveMode ()`
- `void fadeToColor (int r, int g, int b, int duration, int delay, bool inOut)`
- `void forceReloadWPFScreen ()`
- `void gadgetActivate (string name)`
- `void gadgetCreateLayout (string filename, bool realize)`
- `void gadgetDebugLines (string name, bool onoff)`
- `void gadgetDumpDisplays ()`
- `void gadgetFlash (string name, bool flash)`
- `void gadgetReal (string name)`
- `void gadgetRealIfNotMP (string name)`
- `void gadgetRefresh (string name)`
- `void gadgetToggle (string name)`
- `void gadgetToggleIfNotMP (string name)`
- `void gadgetUnreal (string name)`
- `void mapQuickAction (string exactUnitName, string action)`
- `void minimapHighlightType (string name, bool enable)`
- `void openFlareType ()`
- `void resourceUnitConstructBuilding (int unitID, string protoUnitName)`
- `void setFlareType ()`
- `void setGameFadeIn (int r, int g, int b, int duration, int delay, bool inOut)`
- `void SetVillagerToGather (int unitID, bool isFish)`
- `void setVillagerToRepair (int unitID)`
- `void showModsScreen ()`
- `void showWinLoseDisplay (string text, string soundfile)`
- `void testKeyTracking (string name, int val)`
- `void toggleDeveloper ()`
- `void toggleExtendedMinimap ()`
- `void toggleFreeCamera ()`
- `void toggleTREchoLog ()`
- `void toggleXSDebugger ()`
- `void uiAcceptOptions ()`
- `void uiAddChatNotification (int fromPlayerID, int toPlayerID, string stringID, int soundSetID)`
- `void uiAddSelectionButtonDown (bool allowToggle)`
- `void uiAddSelectionButtonUp ()`
- `void uiAddSelectNumberGroup (int group)`
- `void uiAgeUpFromAnywhere ()`
- `void uiApplyLightingSet (int n)`
- `void uiAutoScoutSelectedUnit (int unitID, bool enable)`
- `void uiBeginClickDrag ()`
- `void uiBeginClickRotate ()`
- `void uiBuildAtPointer ()`
- `void uiBuildAtSite ()`
- `void uiBuildWallAtPointer (bool addWaypoint)`
- `void uiCameraControl (float x, float y)`
- `void uiCancelRadialMenu ()`
- `void uiCancelReleasedRadialMenu ()`
- `void uiCancelSelectedBuilding ()`
- `void uiCancelTribute ()`
- `void uiCenterPointer ()`
- `void uiChatDisplayModeToggle ()`
- `void uiChatDisplayModeToHistory ()`
- `void uiChatDisplayModeToRecent ()`
- `void uiChatScrollBack (int keyState)`
- `void uiChatScrollForward (int keyState)`
- `void uiClearChat (bool clearOnly)`
- `void uiClearCursor ()`
- `void uiClearGatherPoint ()`
- `void uiClearMenu (string name)`
- `void uiClearNumberGroup (int group)`
- `void uiClearSelection ()`
- `void uiClearTribute ()`
- `void uiCloseControlsPopup ()`
- `void uiCloseDialog ()`
- `void uiCloseFieldSet ()`
- `void uiConfirmAndLoadQuickSave (string fileName)`
- `void uiControlGroupsPress ()`
- `void uiControlGroupsRelease ()`
- `void uiControlSelectionButtonDown ()`
- `void uiControlSelectionButtonUp ()`
- `void uiCreateNumberGroup (int group)`
- `void uiCycleCurrentActivate ()`
- `void uiCycleGadget (int delta)`
- `void uiDebugConnectivityCacheSetLoginStatus (bool status)`
- `void uiDebugConnectivityCacheSetOnlineStatus (bool status)`
- `void uiDebugConnectivityCacheUseDummyStatus (bool enabled)`
- `void uiDeleteAllSelectedUnits ()`
- `void uiDeleteCameraStartLoc ()`
- `void uiDeleteSelectedUnit ()`
- `void uiDeselectAllOfTarget ()`
- `void uiDeselectTarget ()`
- `void uiDoubleClickDeselect ()`
- `void uiDoubleClickSelect (int add, bool checkAction)`
- `void uiDumpAllUnitHotKeyMappings ()`
- `void uiDumpInputContexts ()`
- `void uiDumpKeyMappings (string context)`
- `void uiDumpUnmappedKeys (string context)`
- `void uiEjectAtPointer ()`
- `void uiEjectBackToWork ()`
- `void uiEjectFromAllMapControlBuildings ()`
- `void uiEjectGarrisonedUnits ()`
- `void uiEmpowerAtPointer ()`
- `void uiEnterContext (string context)`
- `void uiExportGrouping ()`
- `void uiExportTriggers ()`
- `void uiFindAllOfSelectedType ()`
- `void uiFindAllOfTwoTypes (string name1, string name2)`
- `void uiFindAllOfTwoTypesAnd (string name1, string name2)`
- `void uiFindAllOfTwoTypesOnScreen (string name, string secondName, bool isBuilding)`
- `void uiFindAllOfTwoTypesOnScreenAnd (string name, string secondName, bool isBuilding)`
- `void uiFindAllOfType (string name)`
- `void uiFindAllOfTypeIdle (string name)`
- `void uiFindAllOfTypeIdle2 (string name)`
- `void uiFindAllOfTypeOnScreen (string name, bool isBuilding)`
- `void uiFindAllOfTypeOnScreenIdle (string name, bool isBuilding)`
- `void uiFindAllOfTypes (string nameListString)`
- `void uiFindAnyOfTypes (string nameListString)`
- `void uiFindGatherersNotGathering ()`
- `void uiFindIdleOrAnyType (string name, bool shiftSelectsAll, bool controlModifier)`
- `void uiFindIdleType (string name, bool shiftSelectsAll, bool controlModifier, bool groupByType)`
- `void uiFindIdleType2 (string name, bool shiftSelectsAll, bool controlModifier, bool groupByType)`
- `void uiFindKeyMapping (string keyname)`
- `void uiFindMenuPress ()`
- `void uiFindMenuRelease ()`
- `void uiFindNextIdleGroupOfType (string name)`
- `void uiFindNextIdleGroupOfType2 (string name)`
- `void uiFindResourceGatherers (string resourceName)`
- `void uiFindTownBellTC ()`
- `void uiFindTwoTypes (string name1, string name2)`
- `void uiFindTwoTypesAnd (string name1, string name2)`
- `void uiFindType (string name)`
- `void uiFlareAtPointer ()`
- `void uiFlareAtUnit (int unitID)`
- `void uiFrontendBlessingsPickerConfirmSelection ()`
- `void uiFrontendChatBrowserClose ()`
- `void uiFrontendChatBrowserSendMessage ()`
- `void uiFrontendChatBrowserToggleRoomOptions ()`
- `void uiFrontendClanCreate ()`
- `void uiFrontendClanJoinChangePage (bool pageForward, bool goToEnd)`
- `void uiFrontendGenericCycleFocusBackward (bool allowLooping)`
- `void uiFrontendGenericCycleFocusForward (bool allowLooping)`
- `void uiFrontendGenericHorizontalScroll (float axisValue)`
- `void uiFrontendGenericHorizontalScrollLeft (int keyState)`
- `void uiFrontendGenericHorizontalScrollRight (int keyState)`
- `void uiFrontendGenericVerticalScroll (float axisValue)`
- `void uiFrontendGenericVerticalScrollDown (int keyState)`
- `void uiFrontendGenericVerticalScrollUp (int keyState)`
- `void uiFrontendGodPickerConfirmSelection ()`
- `void uiFrontendGodPickerCycleGod (bool nextGod)`
- `void uiFrontendGodsPageToggleLegend ()`
- `void uiFrontendMainMenuNextTab ()`
- `void uiFrontendMainMenuPreviousTab ()`
- `void uiFrontEndMainMenuTab (int tab)`
- `void uiFrontendMatchHistoryChangePage (bool pageForward)`
- `void uiFrontendMPBrowseOpenFilters ()`
- `void uiFrontendMPBrowseRefreshGames ()`
- `void uiFrontendMPRankedSetupBack ()`
- `void uiFrontendMPRankedSetupBeginSearch (bool allowToggle)`
- `void uiFrontendMPRankedSetupCancel ()`
- `void uiFrontendNavigateBack ()`
- `void uiFrontendNotificationsDismissAll ()`
- `void uiFrontendOpenNotificationPanel (bool allowToggle)`
- `void uiFrontEndReportSelectedGame ()`
- `void uiFrontendReportSend ()`
- `void uiFrontendReturnToMPLobby ()`
- `void uiFrontendSkirmishCancelCountdown ()`
- `void uiFrontendSkirmishLeaveLobby ()`
- `void uiFrontendSkirmishReadyToggle ()`
- `void uiFrontendToggleChatBrowser (bool allowToggle)`
- `void uiFrontendToggleHamburgerDropdown (bool allowToggle)`
- `void uiFrontendToggleMinimisedMPLobby ()`
- `void uiFrontendToggleSocialDropdown (bool allowToggle)`
- `void uiFrontendToggleSocialSidebar (bool allowToggle)`
- `void uiFtueBack ()`
- `void uiFtueContinue ()`
- `void uiGamepadLBDown ()`
- `void uiGamepadLBUp ()`
- `void uiGamepadRBDown ()`
- `void uiGamepadRBUp ()`
- `void uiGarrisonToPointer ()`
- `void uiGenericAltPress ()`
- `void uiGodPowersPress ()`
- `void uiGodPowersRelease ()`
- `void uiGuardAtPointer ()`
- `void uiHandleIdleBanner (string name, bool groupByType)`
- `void uiHandleTrainingPanelAction (int unitID, int actionType, int actionID, int actionIdx)`
- `void uiHandleUserTab (int parent)`
- `void uiHideCursor (bool hide)`
- `void uiHotkeyToggleObjectivesDialog ()`
- `void uiIgnoreNextKey ()`
- `void uiImportTriggers ()`
- `void uiLeaveContext (string context)`
- `void uiLeaveModeOnUnshift ()`
- `void uiLetterbox (int on)`
- `void uiLoadSavePopupDelete ()`
- `void uiLoadSavePopupOpenDirectory ()`
- `void uiLoadSavePopupSave ()`
- `void uiLoadTriggers (string filename)`
- `void uiLookAtAndSelectUnit (int lID)`
- `void uiLookAtBattle (int bID)`
- `void uiLookAtNumberGroup (int number)`
- `void uiLookAtProto (string protoname)`
- `void uiLookAtSelection ()`
- `void uiLookAtUnit (int lID)`
- `void uiLTCancelRadialMenu ()`
- `void uiLTSelectRadialMenuEntry ()`
- `void uiMessageBox (string text, string command)`
- `void uiMinimapEnlarge ()`
- `void uiMinorGodUI (int techID, int tcID, int playerID, bool preQueue)`
- `void uiMinorGodUIInSelected (bool preQueue)`
- `void uiMoveAllMilitaryAtPointer ()`
- `void uiMoveAllUnitOfTypeToUnitLocation (int targetUnitID, string typeNames)`
- `void uiMoveUnitOfNameToUnitLocation (int targetUnitID, string unitNames, float minDistance)`
- `void uiMoveUnitOfTypeToUnitLocation (int targetUnitID, string typeNames, float minDistance, bool doWorkOnUnit)`
- `void uiMoveUnitsToPointer (int number, string type)`
- `void uiMPFilterPopupApply ()`
- `void uiMPFilterPopupReset ()`
- `void uiMPHostPopupHostGame ()`
- `void uiMPQuickMatchStartSearch ()`
- `void uiNorseBuildAtSite ()`
- `void uiObjectivesPopupChangeTab (bool nextTab)`
- `void uiObjectivesPopupToggleHints ()`
- `void uiObjectivesPopupToggleObjectivesDisplay ()`
- `void uiOpenChatMenu ()`
- `void uiOpenDiplomacyMenu ()`
- `void uiOpenGameSettings ()`
- `void uiOpenRecordGameBrowser ()`
- `void uiOpenScenarioBrowser (string fileName)`
- `void uiPatrolAtPointer ()`
- `void uiPayFoundation (int unitID)`
- `void uiPopupAccept ()`
- `void uiPopupCancel ()`
- `void uiPostgameAchievementsGoodGame ()`
- `void uiPostgameAchievementsSkipToOverview ()`
- `void uiPostgameChangeTab (bool tabRight)`
- `void uiPostgameClosePopups ()`
- `void uiPostgameLeave ()`
- `void uiPostgameStatisticsChangeTab (bool tabRight)`
- `void uiPostgameViewMap ()`
- `void uiPrimaryContextualButtonDoublePress (bool add)`
- `void uiPrimaryContextualButtonDown ()`
- `void uiPrimaryContextualButtonUp ()`
- `void uiQuickActionChangeToDefault ()`
- `void uiQuickActionCycleLeft ()`
- `void uiQuickActionCycleRight ()`
- `void uiQuickActionNullOp ()`
- `void uiQuickActionToggleAutoBuild ()`
- `void uiQuickSelectDown (bool leftTrigger, bool rightTrigger, bool leftBumper, bool rightBumper)`
- `void uiQuickSelectLeft (bool leftTrigger, bool rightTrigger, bool leftBumper, bool rightBumper)`
- `void uiQuickSelectRight (bool leftTrigger, bool rightTrigger, bool leftBumper, bool rightBumper)`
- `void uiQuickSelectUp (bool leftTrigger, bool rightTrigger, bool leftBumper, bool rightBumper)`
- `void uiQuickTopButtonActionDown ()`
- `void uiQuickTopButtonActionUp (bool allowQuickActionAction)`
- `void uiRadialMenuAltAction ()`
- `void uiRadialMenuChangePage ()`
- `void uiRadialMenuThumbAction ()`
- `void uiRadialMenuViewAction ()`
- `void uiRadialMenuXAxis (float val)`
- `void uiRadialMenuYAxis (float val)`
- `void uiRefreshCommandPanel ()`
- `void uiReleaseDownKeys ()`
- `void uiReleaseQuickSelectDown ()`
- `void uiReleaseQuickSelectLeft ()`
- `void uiReleaseQuickSelectRight ()`
- `void uiReleaseQuickSelectUp ()`
- `void uiReleaseRadialMenuAltAction ()`
- `void uiReleaseRadialMenuEntry ()`
- `void uiRemoveFromAnyNumberGroup ()`
- `void uiRemoveSelectionButtonDown (bool isModified)`
- `void uiRemoveSelectionButtonUp ()`
- `void uiRepairAtPointer ()`
- `void uiResetAllBindings ()`
- `void uiResetCameraOrientation ()`
- `void uiResetCurrentBinding ()`
- `void uiResetInGameCameraRotation ()`
- `void uiResetInGameCameraZoom ()`
- `void uiResetPageOptions ()`
- `void uiSaveAsScenarioBrowser ()`
- `void uiSaveScenarioBrowser ()`
- `void uiSaveScenarioPrompt (bool saveAs)`
- `void uiSaveTriggers (string fn)`
- `void uiScenarioLoad ()`
- `void uiScenarioTestMainMenu ()`
- `void uiScrollChatPanelAxis (float axisValue)`
- `void uiSecondaryContextualButtonDown ()`
- `void uiSecondaryContextualButtonUp ()`
- `void uiSeekShelter ()`
- `void uiSelectAgeUpGod (bool left)`
- `void uiSelectionButtonDown ()`
- `void uiSelectionButtonUp ()`
- `void uiSelectNextUnitStack (bool reverse)`
- `void uiSelectNumberGroup (int group)`
- `void uiSelectRadialMenuEntry ()`
- `void uiSelectTransportUnit ()`
- `void uiSelectType (string nameListString, bool selectAll, bool snapTo, bool forbidSnap)`
- `void uiSendInGameChatMessage (bool closeChat)`
- `void uiSendTribute ()`
- `void uiSetBuildingPlacementRender (int placeID, bool set)`
- `void uiSetCameraStartLoc ()`
- `void uiSetClickDragParams (float deadZoneSize, float maxZoneSize, float exponent, float maxSpeed)`
- `void uiSetGatherPointAtPointer (bool waterSpawnPoint)`
- `void uiSetGatherPointAtPointerOfNearbyUnitTypes (string targetTypes, float maximumDistance, bool waterSpawnPoint)`
- `void uiSetGatherPointAtPointerOfNearbyUnitTypesToUnit (int targetUnitID, string targetTypes, float maximumDistance, bool waterSpawnPoint)`
- `void uiSetKBArmyRender (int armyID, bool set)`
- `void uiSetKBAttackRouteRender (int routeID, bool set)`
- `void uiSetKBResourceRender (int resID, bool set)`
- `void uiSetNearestUnitNamedToBuild (int buildingUnitID, string unitNames)`
- `void uiSetProtoCursor (string proto, bool setPlacement)`
- `void uiSetProtoCursorID (int protoID)`
- `void uiSetProtoID (int id)`
- `void uiSetTerrainDetailPaintMode (int mode)`
- `void uiShowAIDebugInfoArea (int areaID, int renderOn)`
- `void uiShowAIDebugInfoAreaGroup (int areaGroupID, int renderOn)`
- `void uiShowAIDebugInfoAttackRoute (int routeID)`
- `void uiShowAIDebugInfoBase (int baseID)`
- `void uiShowAIDebugInfoEscrow (int id)`
- `void uiShowAIDebugInfoKBArmy (int id)`
- `void uiShowAIDebugInfoKBResource (int resID)`
- `void uiShowAIDebugInfoKBUnit (int state)`
- `void uiShowAIDebugInfoKBUnitPick (int id)`
- `void uiShowAIDebugInfoPlacement (int placeID)`
- `void uiShowAIDebugInfoPlan (int planID)`
- `void uiShowCameraStartLoc ()`
- `void uiShowChatWindow ()`
- `void uiShowEconomicUI ()`
- `void uiShowHelpPopupHistoryTopic (string topicName)`
- `void uiShowMilitaryUI ()`
- `void uiSnapCameraToSelected ()`
- `void uiSocketBuild (int unitID)`
- `void uiSpewDownKeys ()`
- `void uiStartScenarioTest ()`
- `void uiStopScenarioTest ()`
- `void uiStopSelectedUnits ()`
- `void uiSwitchControlsPopup (bool nextPage)`
- `void uiSwitchToGamepadMode ()`
- `void uiSwitchToMouseMode (bool useKeyboard)`
- `void uiTestKeyMapping ()`
- `void uiToggleGarrisonMode ()`
- `void uiToggleSelectionButton ()`
- `void uiToggleUI ()`
- `void uiTransformSelectedUnit (string protoName, bool forceFullyBuilt, int unitID, bool placementPlayer)`
- `void uiTriggerResetParameters ()`
- `void uiTriggerResetSounds ()`
- `void uiTriggerSelectLocation ()`
- `void uiUnbindCurrentBinding ()`
- `void uiUnbuildSelectedUnit ()`
- `void uiUnbuildSelectedUnitAtPointer ()`
- `void uiUnitCommandsMenuPress ()`
- `void uiUnitCommandsMenuRelease ()`
- `void uiUserControls (int on)`
- `void uiVillagerPrioritiesPress ()`
- `void uiVillagerPrioritiesRelease ()`
- `void uiVillagerReturnResources (int targetUnitID, float range)`
- `void uiWheelRotate (int amount)`
- `void uiWheelRotateCamera (int amount)`
- `void uiWheelRotatePlacedUnit (int amount)`
- `void uiWorkAtPointer (int mode)`
- `void uiZoomToProto (string protoname)`
- `void wpfNavigateFrame (string pageUri, string frameName)`

</details>

<details><summary>kbfuncs_8cpp.html (32 declarations)</summary>

- `bool kbAreaGroupsArePassableByLand (int areaGroupID1, int areaGroupID2)`
- `bool kbAttackRouteCreatePaths (int routeID)`
- `bool kbCanSimPath (vector pointA, vector pointB, int unitTypeID, float range)`
- `bool kbGetAutoBaseCreate ()`
- `bool kbGetAutoBaseDetect ()`
- `bool kbResourceGetBlacklisted (int resourceID)`
- `float kbBaseGetOffenseRating (int playerID, int baseID)`
- `float kbGetAutoBaseCreateDistance ()`
- `float kbGetAutoBaseDetectDistance ()`
- `float kbProtoUnitGetLOS (int protoUnitID)`
- `float kbUnitCostPerResource (int protoUnitID, int resourceID)`
- `float kbUnitGetActionDamageForType (int unitID, string actionName, int damageTypeID, bool addBuffs)`
- `float kbUnitGetActionMaximumRange (int unitID, string actionName)`
- `float kbUnitGetActionStatFloat (int unitID, string actionName, int statEnumID)`
- `float kbUnitGetCurrentAICost (int unitID)`
- `float kbUnitGetMaximumAICost (int unitID)`
- `float[] kbUnitGetCost (int protoUnitID)`
- `int kbFindBestBuildingToRepair (vector position, float distance, float healthRatio, int repairUnderAttackUnitTypeID)`
- `int kbUnitGetActionID (int unitID)`
- `int kbUnitGetActionIDByIndex (int unitID, int index)`
- `int kbUnitGetActionTypeByIndex (int unitID, int index)`
- `int kbUnitGetMovementType (int unitTypeID)`
- `int kbUnitGetResourceID (int unitID)`
- `void kbBaseGetMaximumResourceDistance (int playerID, int baseID)`
- `void kbBaseSetMaximumResourceDistance (int playerID, int baseID, float v)`
- `void kbResourceSetBlacklisted (int resourceID, bool toggle)`
- `void kbSetAutoBaseCreate (bool v)`
- `void kbSetAutoBaseCreateDistance (float distance)`
- `void kbSetAutoBaseDetect (bool v)`
- `void kbSetAutoBaseDetectDistance (float distance)`
- `void kbSetAutoBaseMerge (bool v)`
- `void kbUnitQuerySetSeeableOnly (int queryID, bool value)`

</details>

<details><summary>kbtechtreefuncs_8cpp.html (2 declarations)</summary>

- `float kbTechCostPerResource (int techID, int resourceID)`
- `int kbTechTreeGetCheapestUnitUpgrade (int protoUnitID, int researcherTypeID)`

</details>

<details><summary>randommapfuncs_8cpp.html (7 declarations)</summary>

- `bool rmAreaDefSetWaterPaintEdges (int areaID, bool paint)`
- `bool rmAreaSetWaterPaintEdges (int areaID, bool paint)`
- `bool rmInitializeForest (int forestID, float baseHeight)`
- `int rmGetPlacedTeam (int index)`
- `void rmObjectiveScreenSetGoal (string string)`
- `void rmObjectiveScreenSetTitle (string string)`
- `void rmReload ()`

</details>

<details><summary>triggerfuncs_8cpp.html (3 declarations)</summary>

- `bool trUnitSetHP (float hp)`
- `float trUnitDistanceToUnit (int unitID)`
- `void trShowDamage (int unitID, string damageLocations, string smokeLocations, string fireLocations)`

</details>

<details><summary>triggerfuncs__mainthread_8cpp.html (1 declarations)</summary>

- `void trUnitForceRandomName ()`

</details>

<details><summary>xsfuncs_8cpp.html (1 declarations)</summary>

- `bool xsExecute (string command)`

</details>

## Retail-only symbols

<details><summary>aifuncs_8cpp.html (22 declarations)</summary>

- `bool aiPlanHasUnitType (int planID, int unitTypeID)`
- `bool aiSetAutoCastForUnit (int unitID, bool state, int abilitySlot)`
- `int aiAddEchoCategory (string categoryName)`
- `int aiPlanGetOutputCategoryID (int planID)`
- `int aiPlanGetUserVariableIndex (int planID, string variableName)`
- `int[] aiUnitGetForbiddenPlanIDs (int unitID)`
- `void aiAddToResourceBreakdown (int resourceID, int resourceSubTypeID, int numberPlans, int baseID, int[] numNeeded, int[] numWanted, int[] numMax, int[] kbResourceIDs)`
- `void aiEchoCategory (int categoryIndex, string text)`
- `void aiPlanRemoveUnitFromAllPlans (int unitID)`
- `void aiPlanResetBaseID (int planID)`
- `void aiPlanSetOutputCategory (int planID, int outputCategoryID)`
- `void aiPlanSetState (int planID, int planState)`
- `void aiSendNotificationFoundNotEnoughFoodFarmGatheringSpots ()`
- `void aiSendNotificationFoundNotEnoughFoodGatheringSpots ()`
- `void aiSendNotificationFoundNotEnoughGoldGatheringSpots ()`
- `void aiSendNotificationFoundNotEnoughWoodGatheringSpots ()`
- `void aiSetDeleteUnitsForbiddenPlans (bool v)`
- `void aiSetEscrowsEnabled (bool v)`
- `void aiUnitAddForbiddenPlanID (int unitID, int planID)`
- `void aiUnitSetRallyPointToPosition (int sourceUnitID, vector position)`
- `void aiUnitSetRallyPointToUnit (int sourceUnitID, int targetUnitID)`
- `void aiUnitSetTactic (int unitID, int tacticDBID)`

</details>

<details><summary>aiplans_8cpp.html (28 declarations)</summary>

- `const int cAttackPlanNaval = 26`
- `const int cAttackPlanNavalAnchorPoint = 25`
- `const int cAttackPlanUnused = 18`
- `const int cAttackPlanUnused2 = 2`
- `const int cAttackPlanUnused3 = 12`
- `const int cAttackPlanUnused4 = 23`
- `const int cDefendPlanNaval = 18`
- `const int cExplorePlanEngageRange = 24`
- `const int cExplorePlanNaval = 26`
- `const int cExplorePlanTargetIDs = 23`
- `const int cExplorePlanTargetUnitTypes = 25`
- `const int cExplorePlanWaterAreaGroupID = 20`
- `const int cFishPlanHandleDamageFrequency = 4`
- `const int cFishPlanLastHandleDamageTime = 5`
- `const int cGarrisonPlanNaval = 4`
- `const int cGarrisonPlanSearchPosition = 3`
- `const int cResearchPlanTransformToPUID = 5`
- `const int cTrainPlanAreaGroupID = 12`
- `const int cTransportPlanAreaGroupIDToCross = 3`
- `const int cTransportPlanDropOffAreaGroupID = 10`
- `const int cTransportPlanDropOffAreaID = 9`
- `const int cTransportPlanDropOffCurrentIndex = 8`
- `const int cTransportPlanGatherAreaGroupID = 6`
- `const int cTransportPlanGatherAreaID = 5`
- `const int cTransportPlanGatherTimeout = 15`
- `const int cTransportPlanInitializedPoints = 11`
- `const int cTransportPlanStartPoint = 1`
- `const int cTransportPlanTeleportMode = 13`

</details>

<details><summary>kbfuncs_8cpp.html (95 declarations)</summary>

- `bool kbAreaGroupBordersAreaGroupID (int areaGroupID, int borderAreaGroupID)`
- `bool kbCanAreaPath (vector pointA, vector pointB, int movementType, float dangerThreshold, bool allowPartialPath, int[] ignoreAreas, bool allowTeleporters)`
- `bool kbDefaultGetProtoStatFlag (int protoUnitID, int flagEnumID)`
- `bool kbGetAutoMyBaseCreation ()`
- `bool kbGetAutoOtherBaseCreation ()`
- `bool kbGodPowerCheckActiveForAnyPlayer (int protoPowerID)`
- `bool kbLocationFogged (vector location)`
- `bool kbPathAreAreaGroupsConnected (int startAreaGroupID, int goalAreaGroupID, int movementType, bool skipPathingCheckOnGoalAreaGroup)`
- `bool kbPlayerGetProtoStatFlag (int playerID, int protoUnitID, int flagEnumID)`
- `bool kbProtoUnitHasTrainCommands (int protoUnitID)`
- `bool kbResourceIsFlagSet (int kbResourceID, int flag)`
- `bool kbUnitGetIsKnockedOut (int unitID)`
- `bool kbUnitGetStatFlag (int unitID, int flagEnumID)`
- `bool kbUnitIsInBuildingChain (int unitID)`
- `bool kbUnitIsTemporaryCharmedUnit (int unitID)`
- `float kbAICostGetUnitCost (int unitID)`
- `float kbBaseGetCloseToEnemyBaseRating (int playerID, int baseID)`
- `float kbBuildingPlacementGetBufferSpace (int bpID)`
- `float kbGetAutoMyBaseCreationDistance ()`
- `float kbGetAutoMyBaseCreationDistanceTC ()`
- `float kbGetAutoOtherBaseCreationDistance ()`
- `float kbGetAutoOtherBaseCreationDistanceTC ()`
- `float kbPlayerGetExtraBuildingEfficiency (int playerID)`
- `float kbPlayerGetTributePenalty (int playerID)`
- `float kbProtoUnitGetActionDamageForType (int playerID, int protoUnitID, string actionName, int damageType)`
- `float kbProtoUnitGetActionMaximumRange (int playerID, int protoUnitID, string action, int type)`
- `float kbProtoUnitGetActionStatFloat (int playerID, int protoUnitID, string actionName, int statEnumID)`
- `float kbProtoUnitGetBuildingChainRadius (int playerID, int protoUnitID)`
- `float kbProtoUnitGetBuildRate (int playerID, int builderPUID, int buildingPUID)`
- `float kbProtoUnitGetPower (int protoUnitID)`
- `float kbProtoUnitGetSiegePower (int protoUnitID)`
- `float kbProtoUnitInitialResource (int protoUnitID, int resourceID)`
- `float kbUnitGetCommandCost (int unitID, int techID, int resourceID)`
- `float kbUnitGetCurrentDamageMultiplier (int unitID, int damageType)`
- `float kbUnitGetCurrentROFMultiplier (int unitID)`
- `float kbUnitGetDistanceToPoint (int unitID, vector point)`
- `float kbUnitGetDistanceToUnit (int unitID, int otherUnitID)`
- `float kbUnitGetPower (int unitID, bool ignoreCurrentHealth)`
- `float kbUnitGetResourceAutoGatherRate (int unitID, int resourceID)`
- `float kbUnitGetSiegePower (int unitID, bool ignoreCurrentHealth)`
- `float kbUnitQueryGetPower (int queryID, bool ignoreCurrentHealth)`
- `float kbUnitQueryGetSiegePower (int queryID, bool ignoreCurrentHealth)`
- `float kbUnitQueryGetUnitAICost (int queryID, bool considerHealth)`
- `float kbUnitsGetPower (int[] unitIDs, bool ignoreCurrentHealth)`
- `float kbUnitsGetSiegePower (int[] unitIDs, bool ignoreCurrentHealth)`
- `int kbAreaGroupGetBorderAreaGroupID (int areaGroupID, int index)`
- `int kbAreaGroupGetNumberBorderAreaGroups (int areaGroupID)`
- `int kbAreaGroupGetNumberTiles (int areaGroupID)`
- `int kbBuildingPlacementGetSocketID (int bpID)`
- `int kbConvertProtoActionDBIDToEntityActionID (int dbid)`
- `int kbGetAnimationID (string animName)`
- `int kbGetTacticDBID (string tacticName)`
- `int kbGodPowerUnderworldInvasionGetEidolonAmount ()`
- `int kbPlayerGetVisible (int playerID)`
- `int kbProtoUnitGetActionStatInt (int playerID, int protoUnitID, string actionName, int statEnumID)`
- `int kbUnitGetAreaGroupID (int unitID)`
- `int kbUnitGetCurAnimationID (int unitID)`
- `int kbUnitGetCurrentQueueSize (int unitID)`
- `int kbUnitGetKBResourceID (int unitID, bool deadIsValid)`
- `int kbUnitGetNumberUsedByPlans (int unitID)`
- `int kbUnitGetQueueItemAtIndex (int unitID, int index)`
- `int kbUnitGetQueueTypeAtIndex (int unitID, int index)`
- `int kbUnitGetState (int unitID)`
- `int kbUnitGetTactic (int unitID)`
- `int kbUnitGetUsedByPlanID (int unitID, int index)`
- `int[] kbAreaGetIDsByPositionAndRange (vector position, float range, int[] validTypes, bool mustBeOnConnectedAreaGroup, int movementType)`
- `int[] kbAreaGroupGetAllLandAreaGroups ()`
- `int[] kbAreaGroupGetUsefulWaterAreaGroups ()`
- `int[] kbGetPlayersThatAreAttackingUsFromUnits (int[] units)`
- `int[] kbPathCreateAreaGroupPath (int startAreaGroupID, int goalAreaGroupID, int movementType, bool skipPathingCheckOnGoalAreaGroup)`
- `int[] kbProtoUnitGetActionIDs (int playerID, int protoUnitID)`
- `string kbActionGetName (int actionID)`
- `string kbProtoUnitGetDisplayName (int playerID, int protoUnitID)`
- `string kbProtoUnitGetIconPath (int playerID, int protoUnitID, int cultureID)`
- `string kbProtoUnitGetLongRollover (int playerID, int protoUnitID)`
- `string kbProtoUnitGetShortRollover (int playerID, int protoUnitID)`
- `vector kbFindClosestPassablePoint (vector startPoint, int movementType, float range)`
- `vector kbUnitGetTruePosition (int unitID)`
- `void kbBuildingPlacementSetInnerRingRange (int bpID, float innerRingRange)`
- `void kbPathRemoveWaypoint (int pathID, int wpIndex)`
- `void kbPlayerSetVisible (int playerID, int visible)`
- `void kbResourceCombineHerdableResourcesAroundUnit (int unitID, float distance)`
- `void kbResourceSetFlag (int kbResourceID, int flag, bool state)`
- `void kbResourceSortTowardsPosition (int kbResourceID, vector position)`
- `void kbSetAutoMyBaseCreation (bool v)`
- `void kbSetAutoMyBaseCreationDistance (float distance)`
- `void kbSetAutoMyBaseCreationDistanceTC (float distance)`
- `void kbSetAutoOtherBaseCreation (bool distance)`
- `void kbSetAutoOtherBaseCreationDistance (float distance)`
- `void kbSetAutoOtherBaseCreationDistanceTC (float distance)`
- `void kbUnitPickSetCounterModeExcludeTypes (int upID, int[] types)`
- `void kbUnitQuerySetConnectedAreaGroupID (int queryID, int areaGroupID, int movementType)`
- `void kbUnitQuerySetExcludeTypes (int queryID, int[] types)`
- `void kbUnitQuerySetIgnorePlayersThatHaveLost (int queryID, bool value)`
- `void kbUnitQuerySetVisibleState (int queryID, int state)`

</details>

<details><summary>kbtechtreefuncs_8cpp.html (18 declarations)</summary>

- `bool kbTechGetType (int techID, int typeID)`
- `bool kbTechIsPreQueued (int techID)`
- `bool kbTechIsQueued (int techID)`
- `float kbTechGetCostPerResource (int techID, int resourceID)`
- `float kbTechGetDataEffectAmount (int techID, int effectIndex)`
- `float kbTechGetDataEffectRelativity (int techID, int effectIndex)`
- `int kbTechGetDataEffectData2 (int techID, int effectIndex)`
- `int kbTechGetDataEffectData3 (int techID, int effectIndex)`
- `int kbTechGetDataEffectData4 (int techID, int effectIndex)`
- `int kbTechGetDataEffectData5 (int techID, int effectIndex)`
- `int kbTechGetDataEffectData6 (int techID, int effectIndex)`
- `int kbTechGetDataEffectTargetID (int techID, int effectIndex)`
- `int kbTechGetDataEffectTargetType (int techID, int effectIndex)`
- `int kbTechGetDataEffectType (int techID, int effectIndex)`
- `int kbTechGetID (string techName)`
- `string kbTechGetDisplayName (int playerID, int techID)`
- `string kbTechGetIconPath (int playerID, int techID, int cultureID)`
- `string kbTechGetRollover (int playerID, int techID)`

</details>

<details><summary>randommapfuncs_8cpp.html (105 declarations)</summary>

- `bool rmAreaAddForestConstraint (int areaID, int constraintID, float bufferDist)`
- `bool rmAreaAddTerrainConstraint (int areaID, int constraintID, float bufferDist)`
- `bool rmAreaDefAddForestConstraint (int areaDefID, int constraintID, float bufferDist)`
- `bool rmAreaDefAddTerrainConstraint (int areaDefID, int constraintID, float bufferDist)`
- `bool rmAreaDefSetCoherenceSquare (int areaDefID, bool useSquareCoherence)`
- `bool rmAreaDefSetEdgePerturbDistance (int areaDefID, float minPerturbDistanceMeters, float maxPerturbDistanceMeters, bool perturbOnMapEdge)`
- `bool rmAreaDefSetOwnerID (int areaID, int ownerID, int ownerIndex)`
- `bool rmAreaDefSetSizeTiles (int areaDefID, int minTiles, int minSuccessTiles)`
- `bool rmAreaDefSetSizeTilesRange (int areaDefID, int minTiles, int maxTiles, int minSuccessTiles)`
- `bool rmAreaDefSetWaterPaintTerrain (int areaDefID, bool paintEdges)`
- `bool rmAreaFindOriginLocClosestToLoc (int areaID, vector loc, float maxDistMeters)`
- `bool rmAreaFindOriginLocFurthestFromLoc (int areaID, vector loc, float maxDistMeters)`
- `bool rmAreaSetCoherenceSquare (int areaID, bool useSquareCoherence)`
- `bool rmAreaSetEdgePerturbDistance (int areaID, float minPerturbDistanceMeters, float maxPerturbDistanceMeters, bool perturbOnMapEdge)`
- `bool rmAreaSetOwnerID (int areaID, int ownerID, int ownerIndex)`
- `bool rmAreaSetPainted (int areaID)`
- `bool rmAreaSetSizeTiles (int areaID, int minTiles, int minSuccessTiles)`
- `bool rmAreaSetSizeTilesRange (int areaID, int minTiles, int maxTiles, int minSuccessTiles)`
- `bool rmAreaSetWaterPaintTerrain (int areaID, bool paintEdges)`
- `bool rmCustomCliffAddObjectToEdgeLayers (int cliffID, int protoID, float weight)`
- `bool rmCustomCliffAddObjectToSideLayers (int cliffID, int protoID, float weight)`
- `bool rmLocGenAddLocBinding (int locID, int otherLocID, float minDist, float maxDist, bool mutual)`
- `bool rmLocGenSetInArea (int locID, int areaID)`
- `bool rmLocGenSetMaxIterations (int maxIterations)`
- `bool rmObjectDefSetBufferType (int objectDefID, int bufferType, float bufferDist)`
- `bool rmObjectDefSetItemPlaceAnywhere (int objectDefID, int itemIdex, bool placeAnywhere)`
- `bool rmObjectDefSetOwnerID (int objectID, int ownerID, int ownerIndex)`
- `bool rmObjectPlaceNearLoc (int objectID, int playerID, vector loc, float maxDist)`
- `bool rmObjectSetBufferType (int objectDefID, int bufferType, float bufferDist)`
- `bool rmObjectSetItemPlaceAnywhere (int objectID, int itemIdex, bool placeAnywhere)`
- `bool rmObjectSetOwnerID (int objectID, int ownerID, int ownerIndex)`
- `bool rmPathDefSetIgnoreStartEndConstraints (int pathDefID, bool ignoreStartEndConstraints)`
- `bool rmPathDefSetOwnerID (int pathID, int ownerID, int ownerIndex)`
- `bool rmPathSetIgnoreStartEndConstraints (int pathID, bool ignoreStartEndConstraints)`
- `bool rmPathSetOwnerID (int pathID, int ownerID, int ownerIndex)`
- `bool rmRevealLocToPlayer (int playerID, vector loc, float revealRadiusMeters, bool square)`
- `bool rmSetDefaultObjectBufferType (int type)`
- `bool rmSetPlacementPlayers (int[] playerIDs)`
- `bool rmSetPlacementTeams (int[] teamIDs)`
- `bool rmWallsSetTypeIndex (int functionTypeIndex)`
- `float rmGetMapSquareMeters ()`
- `int rmAreaDefGetNumberCreatedAreas (int areaDefID)`
- `int rmAreaDefGetOwnerID (int areaID)`
- `int rmAreaDefGetOwnerIndex (int areaID)`
- `int rmAreaGetOwnerID (int areaID)`
- `int rmAreaGetOwnerIndex (int areaID)`
- `int rmCameraTrackAddWaypoint (int trackIdx, vector position, vector forward, vector up, vector right, float fov)`
- `int rmCameraTrackCreate (string trackName, float durationMs)`
- `int rmClassCreate (string name)`
- `int rmClassGetNumberAreas (int classID)`
- `int rmClassGetNumberAreaTiles (int classID)`
- `int rmClassGetNumberObjects (int classID)`
- `int rmClassGetNumberPaths (int classID)`
- `int rmCreateMultiLocDistanceConstraint (vector[] locs, float minDist, string name)`
- `int rmCreateMultiLocMaxDistanceConstraint (vector[] locs, float maxDist, string name)`
- `int rmCustomCliffGetID (string name)`
- `int rmCustomForestGetID (string name)`
- `int rmCustomMixGetID (string name)`
- `int rmGetMapTiles ()`
- `int rmGetNumberPlayerLocs (int playerID)`
- `int rmGetPlayerLocID (int playerID, int locIdx)`
- `int rmGetPlayerLocOwner (int locID)`
- `int rmGetPlayerLocOwnerIndex (int locID)`
- `int rmLocGenGetLocArea (int locID)`
- `int rmLocGenGetLocObject (int locID)`
- `int rmLocGenGetLocOwnerIndex (int locID)`
- `int rmObjectDefGetOwnerID (int objectID)`
- `int rmObjectDefGetOwnerIndex (int objectID)`
- `int rmObjectGetNumberItems (int objectID)`
- `int rmObjectGetOwnerID (int objectID)`
- `int rmObjectGetOwnerIndex (int objectID)`
- `int rmObjectGetUnitTargetCount (int objectID, int itemIdx)`
- `int rmPathAddRandomWaypoint (int pathID, float minDistFromPreviousMeters, float maxDistFromPreviousMeters)`
- `int rmPathDefAddRandomWaypoint (int pathDefID, float minDistFromPreviousMeters, float maxDistFromPreviousMeters)`
- `int rmPathDefGetNumberCreatedPaths (int pathDefID)`
- `int rmPathDefGetOwnerID (int pathID)`
- `int rmPathDefGetOwnerIndex (int pathID)`
- `int rmPathGetOwnerID (int pathID)`
- `int rmPathGetOwnerIndex (int pathID)`
- `int[] rmAreaDefCreateAndBuildAreas (int areaDefID, int numAreas, bool doPaint, bool buildConcurrently)`
- `int[] rmClassGetAreas (int classID)`
- `int[] rmClassGetObjects (int classID)`
- `int[] rmClassGetPaths (int classID)`
- `int[] rmComputePlayersForPlacement (bool reroll)`
- `int[] rmObjectDefPlaceNearLoc (int objectDefID, int playerID, vector loc, float maxDist, int count)`
- `int[] rmObjectGetCreatedUnitIDs (int objectID, int itemIdx, bool includeRemovedUnitIDs)`
- `string rmCustomCliffGetName (int cliffID)`
- `string rmCustomForestGetName (int forestID)`
- `string rmCustomMixGetName (int mixID)`
- `vector rmGetPlayerLocByID (int locID)`
- `vector rmObjectGetCentroidLoc (int objectID)`
- `vector[] rmAreaGetTiles (int areaID, int type, int[] constraints)`
- `vector[] rmPathGetWaypoints (int pathID)`
- `void rmCameraTrackWaypointSetBias (int trackIdx, int waypointIdx, float bias)`
- `void rmCameraTrackWaypointSetContinuity (int trackIdx, int waypointIdx, float continuity)`
- `void rmCameraTrackWaypointSetTension (int trackIdx, int waypointIdx, float tension)`
- `void rmCameraTrackWaypointSetTime (int trackIdx, int waypointIdx, float timeMs)`
- `void rmRestart ()`
- `void rmSetCanSeeAllyLOSInFFA (bool canSee)`
- `void rmSetDefaultTreeType (int treeProtoID)`
- `void rmSummarySetGoal (string goalText)`
- `void rmSummarySetSpotlightHeader (string titleText)`
- `void rmSummarySetSpotlightImage (string path)`
- `void rmSummarySetSpotlightText (string titleText)`
- `void rmSummarySetTitle (string titleText)`

</details>

<details><summary>triggerfuncs_8cpp.html (100 declarations)</summary>

- `bool trAnythingIsSelected ()`
- `bool trArmyAddUnitTypeInArea (string srcArmy, string unitType, int centerUnit, float radius, bool clearExisting)`
- `bool trCounterAddString (string name, string message)`
- `bool trCounterSetManualString (string name, string message)`
- `bool trIsInBuildingChain (int unitID)`
- `bool trPlayerUnitPerformsActionOnUnit (int playerID, string unitTypeName, string actionName, string targetUnitTypeName)`
- `bool trSetFoundationComplete (int unitID, float pctComplete)`
- `bool trSetGenerateSpirit (int playerID, bool generateSpirit)`
- `bool trTeleportAreaUnitsToTargetArea (int playerID, string unitTypeName, int fromUnitID, float fromUnitRange, int targetUnitID, float targetUnitRange)`
- `bool trUnitFullyBuilt ()`
- `bool trUnitMoveFromAreaToDirection (float x, float y, float z, int eventID, bool bAttackMove, int playerID, string unitType, float radius)`
- `bool trUnitRotateX (int degrees, bool disableTying)`
- `bool trUnitRotateY (int degrees, bool disableTying)`
- `bool trUnitRotateZ (int degrees, bool disableTying)`
- `bool trUnitTypeIsHovered (string proto)`
- `float trPlayerGetCombatXP (int player)`
- `float trTributeReceived (int playerID, int resourceID)`
- `float trUnitShieldPercentDamaged ()`
- `int trCameraTrackAddWaypoint (int trackIdx, vector position, vector forward, vector up, vector right, float fov)`
- `int trCameraTrackCreate (string trackName, float durationMs)`
- `int trGetBloodGroupID (string bloodGroupName)`
- `int trGetImpactEffectID (string impactEffectPath)`
- `int trPlayerGetCombatXPTier (int player)`
- `int trSpawnBloodAtPosition (vector position, float scale, int bloodGroupID)`
- `int trSpawnBloodAtUnit (int unitID, bool preferSplat)`
- `int trSpawnSkeletonAtPosition (vector position, int bloodGroupID)`
- `int trSpawnSkeletonAtUnit (int unitID)`
- `int trUnitGetPlayerID ()`
- `int trUnitGetPlayerIDByUnitID (int unitID)`
- `int trUnitNumberSelected ()`
- `string trFormatString (string format, string[] inserts)`
- `string trGetNameForBloodGroupID (int bloodGroupID)`
- `void trAreaUnitHighlight (int playerID, float duration, string unitType, int centerUnit, float radius)`
- `void trAreaUnitTask (int playerID, int destUnitID, string unitType, int centerUnit, float radius, int event)`
- `void trBoxFormationScale (float scale)`
- `void trBoxFormationSpacing (float minUnitRadius)`
- `void trCameraAttachToUnitPerspective (bool bEnable)`
- `void trCameraAttachToUnitPerspectiveByUnitID (bool bEnable, int unitID)`
- `void trCameraCutToUnit ()`
- `void trCameraSetOverridePlayerCanExit (bool canLeaveCamera)`
- `void trCameraTrackWaypointSetBias (int trackIdx, int waypointIdx, float bias)`
- `void trCameraTrackWaypointSetContinuity (int trackIdx, int waypointIdx, float continuity)`
- `void trCameraTrackWaypointSetTension (int trackIdx, int waypointIdx, float tension)`
- `void trCameraTrackWaypointSetTime (int trackIdx, int waypointIdx, float timeMs)`
- `void trCameraUnitPerspectiveSetAttachPoint (string attachPointName)`
- `void trConvertUnitsInAreaLimited (int centerUnit, int srcPlayer, int trgPlayer, string unitTypeName, float range, int maxUnits)`
- `void trCounterAddVictory (string name, int start, int stop, string message, int playerID, int eventID)`
- `void trCounterAddVictoryMs (string name, int start, int stop, string message, int playerID, int eventID)`
- `void trCounterSetSpecialType (string name, int value)`
- `void trCounterTimeDecrement (string name, int value)`
- `void trCounterTimeIncrement (string name, int value)`
- `void trDespawnAllBlood (bool fadeOut, bool forceRapid)`
- `void trDespawnAllBloodAt (vector position, float radius, bool fadeOut, bool forceRapid, bool ignoreVisibility)`
- `void trDespawnAllBloodByBloodPoolID (int bloodManagerID, bool fadeOut, bool forceRapid, bool ignoreVisibility)`
- `void trDespawnAllSkeletons (bool fadeOut, bool forceRapid)`
- `void trDespawnAllSkeletonsAt (vector position, float radius, bool fadeOut, bool forceRapid, bool ignoreVisibility)`
- `void trDespawnAllSkeletonsByBloodManagerID (int bloodManagerID, bool fadeOut, bool forceRapid, bool ignoreVisibility)`
- `void trExecuteConsoleCommand (string command)`
- `void trForceShowObjectivePanel (bool value)`
- `void trGodPowerAddExtraFreeCharges (int playerID, string protoPowerName, int numUses)`
- `void trLightingSetParamBool (int paramID, bool value)`
- `void trLightingSetParamColor (int paramID, int r, int g, int b)`
- `void trLightingSetParamColorAttr (int paramID, float redAttr, float greenAttr, float blueAttr)`
- `void trLightingSetParamFloat (int paramID, float value)`
- `void trLightingSetParamInt (int paramID, int value)`
- `void trModifyProtounitUnitType (string unitTypeName, string trgUnitTypeName, int playerID, int puField, float delta, int relativity)`
- `void trPlaceStartingUnits (int playerID)`
- `void trPlayerAllowBonusUnitSpawning (int playerID, bool allowSpawning)`
- `void trPlayerEnableBuildingChain (int playerID, bool enable)`
- `void trPlayerEnableCombatXP (int playerID, bool enable)`
- `void trPlayerGrantCombatXP (int player, float amount)`
- `void trPlayerSetCombatXPTier (int player, int tier)`
- `void trPlayerSetMaxCombatXPTier (int player, int maxTier)`
- `void trPlayerTimeshiftModifyTimeRatio (int playerID, string protoName, float delta, int relativity)`
- `void trProtounitActionSetFlag (int playerID, string unitTypeName, string actionName, string actionFlag, bool set)`
- `void trProtounitAssignAction (string unitTypeName, string protoUnitName, string actionName, int playerID)`
- `void trProtounitModifyReplacementData (string unitTypeName, int playerID, string replProtoName, int eventType, float delta, int relativity)`
- `void trProtounitModifySpawnData (string unitTypeName, int playerID, string spawnProtoName, int eventType, float delta, int relativity, float chance, float lifespan)`
- `void trProtounitVeterancyAddRank (string unitTypeName, int playerID, int rankTypeID, float value)`
- `void trProtounitVeterancyBonus (string unitTypeName, int playerID, int rankID, int modifyType, int damageType, float delta, int relativity)`
- `void trSetCanSeeAllyLOSInFFA (bool canSee, bool applyFogChangeNow)`
- `void trSetCommunityObjectivesVisibility (bool show)`
- `void trSetCounterDisplayWithType (string message, int specialCounterType)`
- `void trSetFavorStashDisabled (bool isDisabled)`
- `void trSetMilitaryAutoTrain (bool locked)`
- `void trSetTeamsLocked (bool locked)`
- `void trSetUniqueCounterDisplay (string name, string message)`
- `void trSetUniqueCounterDisplayWithType (string name, string message, int specialCounterType)`
- `void trSpawnBloodAtSelectedUnits (bool preferSplat)`
- `void trSpawnBloodHitVFXAtPosition (vector position, int impactEffectID, int impactEffectTypeID, int bloodPoolGroupID)`
- `void trSpawnBloodHitVFXAtSelectedUnits (int impactEffectID)`
- `void trSpawnBloodHitVFXAtUnit (int unitID, int impactEffectID)`
- `void trSpawnSkeletonsAtSelectedUnits ()`
- `void trUnitSetFlag (int flagID, bool set)`
- `void trUnitSetShieldPoints (float value)`
- `void trUnitSetVisualProperty (int propertyTypeID, vector targetVector, int terrainVFXAppearanceTypeID, int terrainVFXTintColor, float terrainVFXWaterBillboardBias, int vfxIconType)`
- `void trUnitSetVisualPropertyParticleIcon (int vfxIconType)`
- `void trUnitSetVisualPropertyParticleTarget (vector targetVector)`
- `void trUnitSetVisualPropertyScaleWithModelTransform ()`
- `void trUnitSetVisualPropertyTerrainProperties (int terrainVFXAppearanceTypeID, int terrainVFXTintColor, float terrainVFXWaterBillboardBias)`

</details>

<details><summary>triggerfuncs__mainthread_8cpp.html (25 declarations)</summary>

- `bool trInGamepadMode ()`
- `bool trInInputContext (string inputContext)`
- `bool trInRadialMenuPage (int radialMenuPageID)`
- `bool trIsMinimapExpanded ()`
- `bool trUnitUseSpecificAbility (int unitID, string abilityName, int targetID, vector position, bool setAsQueued)`
- `void trChatClearHudMessages ()`
- `void trChatKeepLastMessagesOnScreen (bool status)`
- `void trClearDialogueSoundEvent ()`
- `void trCreateUnitNumberGroup (int group)`
- `void trLoadCustomResource (string resourcePath)`
- `void trLockGodPower (int slotIdx, bool locked, int playerIdx)`
- `void trSetBuildingChainVisible (int playerID, bool visibile, bool force)`
- `void trSetDialogueSoundEvent (string name)`
- `void trSetVictoryPlayers (int[] playerList)`
- `void trShowHidePopup (int type, bool display)`
- `void trTutorialEndChoice ()`
- `void trUIBlockMinimapExpansion (bool blocked)`
- `void trUIBlockRadialMenu (int menuIndex, bool display)`
- `void trUIFlashAbility (string puCmdName, bool flash)`
- `void trUIFlashAgeUp (bool flash)`
- `void trUIFlashGodPowerAll (bool flash)`
- `void trUIForceLockGodPowerSlot (int slotIdx, bool forceDisable)`
- `void trUIGamepadPromptFlash (int promptIndex, bool flash)`
- `void trUIGamepadPromptVisibility (int promptIndex, bool display)`
- `void trUIHideRadialMenuPromptPanel (bool hidden)`

</details>

<details><summary>xsfuncs_8cpp.html (5 declarations)</summary>

- `float clamp (float val, float minVal, float maxVal)`
- `void xsSetRuleMaxIntervalMS (string ruleName, int maxIntervalMS)`
- `void xsSetRuleMaxIntervalSelfMS (int maxIntervalMS)`
- `void xsSetRuleMinIntervalMS (string ruleName, int minIntervalMS)`
- `void xsSetRuleMinIntervalSelfMS (int minIntervalMS)`

</details>

## Shared names with different declarations

<details><summary>Compare declarations</summary>

| Symbol | Older declaration | Retail declaration |
| --- | --- | --- |
| `abs` | `float abs (float _X)` | `float abs (float x)` |
| `acos` | `float acos (float _X)` | `float acos (float x)` |
| `aiCastGodPowerAtPosition` | `bool aiCastGodPowerAtPosition (int protoPowerID, vector position, bool setAsQueued)` | `bool aiCastGodPowerAtPosition (int protoPowerID, vector position)` |
| `aiCastGodPowerAtUnit` | `bool aiCastGodPowerAtUnit (int protoPowerID, int unitID, bool setAsQueued)` | `bool aiCastGodPowerAtUnit (int protoPowerID, int unitID)` |
| `aiChat` | `void aiChat (int playerID, string text)` | `void aiChat (int playerID, string chatString)` |
| `aiCommsSendStatement` | `void aiCommsSendStatement (int targetPlayerID, int promptType)` | `void aiCommsSendStatement (int playerID, int promptType)` |
| `aiCommsSendStatementWithVector` | `void aiCommsSendStatementWithVector (int targetPlayerID, int promptType, vector position)` | `void aiCommsSendStatementWithVector (int playerID, int promptType, vector position)` |
| `aiCommsSetEventHandler` | `void aiCommsSetEventHandler (string handlerName)` | `void aiCommsSetEventHandler (string handlerFunctionName)` |
| `aiGetNumberGatherers` | `int aiGetNumberGatherers (int gathererPUID, int resourceID, int resourceSubTypeID, int resourcePUID)` | `int aiGetNumberGatherers (int gathererPUID, int resourceID, int resourceSubType, int resourcePUID)` |
| `aiPlanAddUnit` | `bool aiPlanAddUnit (int planID, int unitID, bool loan)` | `bool aiPlanAddUnit (int planID, int unitID)` |
| `aiPlanAddUserVariableBool` | `void aiPlanAddUserVariableBool (int planID, int variableIndex, string variableName, int numberValues)` | `void aiPlanAddUserVariableBool (int planID, int variableIndex, string name, int numberValues)` |
| `aiPlanAddUserVariableFloat` | `void aiPlanAddUserVariableFloat (int planID, int variableIndex, string variableName, int numberValues)` | `void aiPlanAddUserVariableFloat (int planID, int variableIndex, string name, int numberValues)` |
| `aiPlanAddUserVariableInt` | `void aiPlanAddUserVariableInt (int planID, int variableIndex, string variableName, int numberValues)` | `void aiPlanAddUserVariableInt (int planID, int variableIndex, string name, int numberValues)` |
| `aiPlanAddUserVariableString` | `void aiPlanAddUserVariableString (int planID, int variableIndex, string variableName, int numberValues)` | `void aiPlanAddUserVariableString (int planID, int variableIndex, string name, int numberValues)` |
| `aiPlanAddUserVariableVector` | `void aiPlanAddUserVariableVector (int planID, int variableIndex, string variableName, int numberValues)` | `void aiPlanAddUserVariableVector (int planID, int variableIndex, string name, int numberValues)` |
| `aiPlanAddWaypoint` | `void aiPlanAddWaypoint (int planID, vector pWayPoint)` | `void aiPlanAddWaypoint (int planID, vector waypoint)` |
| `aiPlanCreate` | `int aiPlanCreate (string planName, int type, int parentPlanID)` | `int aiPlanCreate (string planName, int type, int parentPlanID, int outputCategoryID)` |
| `aiPlanDestroy` | `bool aiPlanDestroy (int planID)` | `void aiPlanDestroy (int planID)` |
| `aiPlanDestroyByName` | `bool aiPlanDestroyByName (string name)` | `void aiPlanDestroyByName (string planName)` |
| `aiPlanGetChildIDByIndex` | `int aiPlanGetChildIDByIndex (int planID, int index)` | `int aiPlanGetChildIDByIndex (int parentPlanID, int index)` |
| `aiPlanGetIDByTypeAndState` | `int aiPlanGetIDByTypeAndState (int planType, int planState, int index, bool active)` | `int aiPlanGetIDByTypeAndState (int planType, int planState, int index)` |
| `aiPlanGetIDByTypeAndVariableIntValue` | `int aiPlanGetIDByTypeAndVariableIntValue (int planType, int varIndex, int variableValue, int index, bool active)` | `int aiPlanGetIDByTypeAndVariableIntValue (int planType, int varIndex, int variableValue, int index)` |
| `aiPlanGetIDByTypeIndex` | `int aiPlanGetIDByTypeIndex (int planType, int index, bool active)` | `int aiPlanGetIDByTypeIndex (int planType, int index)` |
| `aiPlanGetIDsByType` | `int[] aiPlanGetIDsByType (int planType, bool active)` | `int[] aiPlanGetIDsByType (int planType)` |
| `aiPlanGetIDsByTypeAndState` | `int[] aiPlanGetIDsByTypeAndState (int planType, int planState, bool active)` | `int[] aiPlanGetIDsByTypeAndState (int planType, int planState)` |
| `aiPlanGetIDsByTypeAndVariableBoolValue` | `int[] aiPlanGetIDsByTypeAndVariableBoolValue (int planType, int varIndex, bool variableValue, bool active)` | `int[] aiPlanGetIDsByTypeAndVariableBoolValue (int planType, int varIndex, bool variableValue)` |
| `aiPlanGetIDsByTypeAndVariableFloatValue` | `int[] aiPlanGetIDsByTypeAndVariableFloatValue (int planType, int varIndex, float variableValue, bool active)` | `int[] aiPlanGetIDsByTypeAndVariableFloatValue (int planType, int varIndex, float variableValue)` |
| `aiPlanGetIDsByTypeAndVariableIntValue` | `int[] aiPlanGetIDsByTypeAndVariableIntValue (int planType, int varIndex, int variableValue, bool active)` | `int[] aiPlanGetIDsByTypeAndVariableIntValue (int planType, int varIndex, int variableValue)` |
| `aiPlanGetIDsByTypeAndVariableStringValue` | `int[] aiPlanGetIDsByTypeAndVariableStringValue (int planType, int varIndex, string variableValue, bool active)` | `int[] aiPlanGetIDsByTypeAndVariableStringValue (int planType, int varIndex, string variableValue)` |
| `aiPlanGetIDsByTypeAndVariableVectorValue` | `int[] aiPlanGetIDsByTypeAndVariableVectorValue (int planType, int varIndex, vector variableValue, bool active)` | `int[] aiPlanGetIDsByTypeAndVariableVectorValue (int planType, int varIndex, vector variableValue)` |
| `aiPlanGetNumberByType` | `int aiPlanGetNumberByType (int planType, bool active)` | `int aiPlanGetNumberByType (int planType)` |
| `aiPlanGetNumberByTypeAndState` | `int aiPlanGetNumberByTypeAndState (int planType, int planState, bool active)` | `int aiPlanGetNumberByTypeAndState (int planType, int planState)` |
| `aiPlanGetNumberByTypeAndVariableIntValue` | `int aiPlanGetNumberByTypeAndVariableIntValue (int planType, int varIndex, int variableValue, bool active)` | `int aiPlanGetNumberByTypeAndVariableIntValue (int planType, int varIndex, int variableValue)` |
| `aiPlanGetNumberChildren` | `int aiPlanGetNumberChildren (int planID)` | `int aiPlanGetNumberChildren (int parentPlanID)` |
| `aiPlanGetUnits` | `int[] aiPlanGetUnits (int planID, int unitTypeID, bool countLoans)` | `int[] aiPlanGetUnits (int planID, int unitTypeID, bool countLoans, int[] excludeTypes)` |
| `aiPlanSetNumberUserVariableValues` | `void aiPlanSetNumberUserVariableValues (int planID, int variableIndex, int numberValues, bool clear)` | `void aiPlanSetNumberUserVariableValues (int planID, int variableIndex, int numberValues, bool clearCurrentValues)` |
| `aiPlanSetUserVariableBool` | `void aiPlanSetUserVariableBool (int planID, int variableIndex, int valueIndex, bool variableValue)` | `void aiPlanSetUserVariableBool (int planID, int variableIndex, int valueIndex, bool value)` |
| `aiPlanSetUserVariableFloat` | `void aiPlanSetUserVariableFloat (int planID, int variableIndex, int valueIndex, float variableValue)` | `void aiPlanSetUserVariableFloat (int planID, int variableIndex, int valueIndex, float value)` |
| `aiPlanSetUserVariableInt` | `void aiPlanSetUserVariableInt (int planID, int variableIndex, int valueIndex, int variableValue)` | `void aiPlanSetUserVariableInt (int planID, int variableIndex, int valueIndex, int value)` |
| `aiPlanSetUserVariableString` | `void aiPlanSetUserVariableString (int planID, int variableIndex, int valueIndex, string variableValue)` | `void aiPlanSetUserVariableString (int planID, int variableIndex, int valueIndex, string value)` |
| `aiPlanSetUserVariableVector` | `void aiPlanSetUserVariableVector (int planID, int variableIndex, int valueIndex, vector variableValue)` | `void aiPlanSetUserVariableVector (int planID, int variableIndex, int valueIndex, vector value)` |
| `aiPlanSetVariableBool` | `void aiPlanSetVariableBool (int planID, int variableIndex, int valueIndex, bool variableValue)` | `void aiPlanSetVariableBool (int planID, int variableIndex, int valueIndex, bool value)` |
| `aiPlanSetVariableFloat` | `void aiPlanSetVariableFloat (int planID, int variableIndex, int valueIndex, float variableValue)` | `void aiPlanSetVariableFloat (int planID, int variableIndex, int valueIndex, float value)` |
| `aiPlanSetVariableInt` | `void aiPlanSetVariableInt (int planID, int variableIndex, int valueIndex, int variableValue)` | `void aiPlanSetVariableInt (int planID, int variableIndex, int valueIndex, int value)` |
| `aiPlanSetVariableString` | `void aiPlanSetVariableString (int planID, int variableIndex, int valueIndex, string variableValue)` | `void aiPlanSetVariableString (int planID, int variableIndex, int valueIndex, string value)` |
| `aiPlanSetVariableVector` | `void aiPlanSetVariableVector (int planID, int variableIndex, int valueIndex, vector variableValue)` | `void aiPlanSetVariableVector (int planID, int variableIndex, int valueIndex, vector value)` |
| `aiSetAttackResponseDistance` | `void aiSetAttackResponseDistance (float distance)` | `void aiSetAttackResponseDistance (float v)` |
| `aiSetDefaultStance` | `void aiSetDefaultStance (int stance)` | `void aiSetDefaultStance (int defaultStance)` |
| `aiSetEconomyPop` | `void aiSetEconomyPop (int pop)` | `void aiSetEconomyPop (int v)` |
| `aiSetExploreDangerThreshold` | `void aiSetExploreDangerThreshold (float threshold)` | `void aiSetExploreDangerThreshold (float value)` |
| `aiSetHandler` | `void aiSetHandler (string handlerName, int type)` | `void aiSetHandler (string handlerName, int eventType)` |
| `aiSetMicroFlags` | `void aiSetMicroFlags (int level)` | `void aiSetMicroFlags (int flags)` |
| `aiSetMilitaryPop` | `void aiSetMilitaryPop (int pop)` | `void aiSetMilitaryPop (int v)` |
| `aiSetMostHatedNavalPlayerID` | `void aiSetMostHatedNavalPlayerID (int playerID)` | `void aiSetMostHatedNavalPlayerID (int v)` |
| `aiSetMostHatedPlayerID` | `void aiSetMostHatedPlayerID (int playerID)` | `void aiSetMostHatedPlayerID (int v)` |
| `aiSetNavalEconomyPop` | `void aiSetNavalEconomyPop (int pop)` | `void aiSetNavalEconomyPop (int v)` |
| `aiSetNavalMilitaryPop` | `void aiSetNavalMilitaryPop (int pop)` | `void aiSetNavalMilitaryPop (int v)` |
| `aiSetOutpostLimit` | `void aiSetOutpostLimit (int v)` | `void aiSetOutpostLimit (int limit)` |
| `aiSetResourceBreakdown` | `void aiSetResourceBreakdown (int resourceID, int resourceSubTypeID, int numberPlans, int planPriority, float percentage, int baseID, int[] numNeeded, int[] numWanted, int[] numMax)` | `void aiSetResourceBreakdown (int resourceID, int resourceSubTypeID, int numberPlans, int planPriority, int baseID, int[] numNeeded, int[] numWanted, int[] numMax, int[] kbResourceIDs)` |
| `aiSetResourcePercentage` | `void aiSetResourcePercentage (int resourceID, bool normalize, float percentage)` | `void aiSetResourcePercentage (int resourceID, float percentage)` |
| `aiSwitchMainBase` | `void aiSwitchMainBase (int newBaseID, bool force)` | `void aiSwitchMainBase (int newBaseID)` |
| `aiTaskBuildUnit` | `bool aiTaskBuildUnit (int unitID, int targetUnitTypeID, vector position, bool queue, int heading)` | `bool aiTaskBuildUnit (int unitID, int buildingTypeID, vector position, bool queue, int heading)` |
| `aiTaskBuildUnits` | `bool aiTaskBuildUnits (int[] units, int targetUnitTypeID, vector position, bool queue, int heading)` | `bool aiTaskBuildUnits (int[] unitIDs, int buildingTypeID, vector position, bool queue, int heading)` |
| `aiTaskDeleteUnits` | `bool aiTaskDeleteUnits (int[] units)` | `bool aiTaskDeleteUnits (int[] unitIDs)` |
| `aiTaskGarrisonUnits` | `bool aiTaskGarrisonUnits (int[] units, int targetID)` | `bool aiTaskGarrisonUnits (int[] unitIDs, int targetID)` |
| `aiTaskMoveUnit` | `bool aiTaskMoveUnit (int unitID, vector position, bool queue)` | `bool aiTaskMoveUnit (int unitID, vector position, bool attackMove, bool queue)` |
| `aiTaskMoveUnits` | `bool aiTaskMoveUnits (int[] units, vector position, bool queue)` | `bool aiTaskMoveUnits (int[] unitIDs, vector position, bool attackMove, bool queue)` |
| `aiTaskStopUnits` | `bool aiTaskStopUnits (int[] units)` | `bool aiTaskStopUnits (int[] unitIDs)` |
| `aiTaskTrainUnit` | `bool aiTaskTrainUnit (int unitID, int targetUnitTypeID)` | `bool aiTaskTrainUnit (int unitID, int unitTypeID)` |
| `aiTaskUngarrisonUnits` | `bool aiTaskUngarrisonUnits (int[] units, vector position)` | `bool aiTaskUngarrisonUnits (int[] unitIDs, vector position)` |
| `aiTaskWorkUnits` | `bool aiTaskWorkUnits (int[] units, int targetUnitID, bool queue)` | `bool aiTaskWorkUnits (int[] unitIDs, int targetUnitID, bool queue)` |
| `aiTransformWallIntoGate` | `void aiTransformWallIntoGate (int wallLongID)` | `bool aiTransformWallIntoGate (int wallLongID)` |
| `asin` | `float asin (float _X)` | `float asin (float x)` |
| `atan` | `float atan (float _X)` | `float atan (float x)` |
| `atan2` | `float atan2 (float _Y, float _X)` | `float atan2 (float y, float x)` |
| `ceil` | `float ceil (float _X)` | `float ceil (float x)` |
| `cos` | `float cos (float _X)` | `float cos (float x)` |
| `floor` | `float floor (float _X)` | `float floor (float x)` |
| `hypot` | `float hypot (float _X, float _Y)` | `float hypot (float x, float y)` |
| `kbAICostGetProtoUnitCost` | `float kbAICostGetProtoUnitCost (int protoUnitTypeID)` | `float kbAICostGetProtoUnitCost (int protoUnitID)` |
| `kbAICostSetWeight` | `bool kbAICostSetWeight (int resourceID, float weight)` | `void kbAICostSetWeight (int resourceID, float weight)` |
| `kbArmyGetUnitID` | `int kbArmyGetUnitID (int armyID, int index)` | `int kbArmyGetUnitID (int armyID, int unitNumber)` |
| `kbArmyRemoveUnitByIndex` | `void kbArmyRemoveUnitByIndex (int armyID, int index)` | `void kbArmyRemoveUnitByIndex (int armyID, int unitIndex)` |
| `kbBaseFindOrCreateResourceBase` | `int kbBaseFindOrCreateResourceBase (vector position, int resourceType, int resourceSubType, float distance, float dangerTreshold, bool unclaimedOnly, bool idleOnly, bool areaGroupsNeedToMatch)` | `int kbBaseFindOrCreateResourceBase (vector position, int resourceType, int resourceSubType, float distance, float dangerThreshold, bool unclaimedOnly, bool idleOnly, bool areaGroupsNeedToMatch)` |
| `kbBaseGetDefenseRating` | `float kbBaseGetDefenseRating (int playerID, int baseID)` | `float kbBaseGetDefenseRating (int playerID, int baseID, bool includeCloseToEnemyBaseRating)` |
| `kbBaseSetFrontVector` | `void kbBaseSetFrontVector (int playerID, int baseID, vector front)` | `void kbBaseSetFrontVector (int playerID, int baseID, vector frontVector)` |
| `kbBuildingPlacementAddPositionInfluence` | `void kbBuildingPlacementAddPositionInfluence (int bpID, vector position, float influenceValue, float influenceDistance, int falloff)` | `void kbBuildingPlacementAddPositionInfluence (int bpID, vector position, float value, float distance, int falloff)` |
| `kbCanPath` | `bool kbCanPath (vector pointA, vector pointB, int unitTypeID, float range)` | `bool kbCanPath (vector pointA, vector pointB, int protoUnitID, float range, int targetID)` |
| `kbCreateAttackRouteWithPath` | `int kbCreateAttackRouteWithPath (string name, vector startPoint, vector endPoint, int numInitialSectors)` | `int kbCreateAttackRouteWithPath (string name, vector startPoint, vector targetPoint)` |
| `kbDefaultGetProtoStatString` | `string kbDefaultGetProtoStatString (int protoUnitID, int stat)` | `string kbDefaultGetProtoStatString (int protoUnitID, int statEnumID)` |
| `kbFindClosestBase` | `int kbFindClosestBase (int playerRelation, vector location, bool militaryOnly)` | `int kbFindClosestBase (int playerID, int playerRelation, vector location, int movementType, bool militaryBasesOnly)` |
| `kbGetAmountValidResourcesByPosition` | `float kbGetAmountValidResourcesByPosition (vector position, int resourceType, int resourceSubType, float distance, float dangerTreshold, bool unclaimedOnly, bool idleOnly, bool areaGroupsNeedToMatch)` | `float kbGetAmountValidResourcesByPosition (vector position, int resourceType, int resourceSubType, float distance, float dangerThreshold, bool unclaimedOnly, bool idleOnly, bool areaGroupsNeedToMatch)` |
| `kbGetCombatEfficiency` | `float kbGetCombatEfficiency (int playerID1, int unitTypeID1, int playerID2, int unitTypeID2, bool ignoreTrainCheck)` | `float kbGetCombatEfficiency (int playerID1, int unitTypeID1, int playerID2, int unitTypeID2, bool ignoreTrainCheck, bool considerCost)` |
| `kbGetNumberValidResourcesByPosition` | `int kbGetNumberValidResourcesByPosition (vector position, int resourceType, int resourceSubType, float distance, float dangerTreshold, bool unclaimedOnly, bool idleOnly, bool areaGroupsNeedToMatch)` | `int kbGetNumberValidResourcesByPosition (vector position, int resourceType, int resourceSubType, float distance, float dangerThreshold, bool unclaimedOnly, bool idleOnly, bool areaGroupsNeedToMatch)` |
| `kbGetPopulationSlotsByUnitTypeID` | `int kbGetPopulationSlotsByUnitTypeID (int unitTypeID, int playerID)` | `int kbGetPopulationSlotsByUnitTypeID (int unitTypeID, int playerID, int state)` |
| `kbGetResourceName` | `string kbGetResourceName (int id)` | `string kbGetResourceName (int resourceID)` |
| `kbGetResourceSelectorFactor` | `float kbGetResourceSelectorFactor (int type, int resourceType)` | `float kbGetResourceSelectorFactor (int type, int resourceID)` |
| `kbGetStatValueFloat` | `float kbGetStatValueFloat (int playerID, int statID, int param)` | `float kbGetStatValueFloat (int playerID, int statTypeID, int param)` |
| `kbGetStatValueInt` | `int kbGetStatValueInt (int playerID, int statID, int param)` | `int kbGetStatValueInt (int playerID, int statTypeID, int param)` |
| `kbGetValidResourcesByPosition` | `int[] kbGetValidResourcesByPosition (vector position, int resourceType, int resourceSubType, float distance, float dangerTreshold, bool unclaimedOnly, bool idleOnly, bool areaGroupsNeedToMatch)` | `int[] kbGetValidResourcesByPosition (vector position, int resourceType, int resourceSubType, float distance, float dangerThreshold, bool unclaimedOnly, bool idleOnly, bool areaGroupsNeedToMatch)` |
| `kbGodPowerGetPrePurchaseCost` | `float kbGodPowerGetPrePurchaseCost (int protoPowerID, int numUses, int playerID)` | `float kbGodPowerGetPrePurchaseCost (int protoPowerID, int playerID, int numUses)` |
| `kbPathAddWaypoint` | `void kbPathAddWaypoint (int pathID, vector wp)` | `void kbPathAddWaypoint (int pathID, vector waypoint)` |
| `kbPathAddWaypointAfter` | `void kbPathAddWaypointAfter (int pathID, int wpIndex, vector wp)` | `void kbPathAddWaypointAfter (int pathID, int waypointIndex, vector waypoint)` |
| `kbPathCreateAreaPath` | `bool kbPathCreateAreaPath (int pathID, int startAreaID, int goalAreaID, int movementType, bool avoidDanger, bool allowPartialPath, bool ignoreForestAreas)` | `bool kbPathCreateAreaPath (int pathID, int startAreaID, int goalAreaID, int movementType, float dangerThreshold, bool allowPartialPath, bool allowTeleporters)` |
| `kbPlayerGetProtoStatString` | `string kbPlayerGetProtoStatString (int playerID, int protoUnitID, int stat)` | `string kbPlayerGetProtoStatString (int playerID, int protoUnitID, int statEnumID)` |
| `kbPlayerSetHandicap` | `void kbPlayerSetHandicap (int playerID, float fHandicap)` | `void kbPlayerSetHandicap (int playerID, float handicap)` |
| `kbProtoUnitIsType` | `bool kbProtoUnitIsType (int protoUnitID, int unitType)` | `bool kbProtoUnitIsType (int protoUnitID, int unitTypeID)` |
| `kbResourceGetClosestDropsiteID` | `int kbResourceGetClosestDropsiteID (int resourceID)` | `int kbResourceGetClosestDropsiteID (int kbResourceID)` |
| `kbResourceGetFarmIDWithFurthestAwayDropsite` | `int kbResourceGetFarmIDWithFurthestAwayDropsite (int resourceID)` | `int kbResourceGetFarmIDWithFurthestAwayDropsite (int kbResourceID)` |
| `kbResourceGetIsIDValid` | `bool kbResourceGetIsIDValid (int resourceID)` | `bool kbResourceGetIsIDValid (int kbResourceID)` |
| `kbResourceGetNumberUnits` | `int kbResourceGetNumberUnits (int resourceID)` | `int kbResourceGetNumberUnits (int kbResourceID)` |
| `kbResourceGetPlanID` | `int kbResourceGetPlanID (int resourceID)` | `int kbResourceGetPlanID (int kbResourceID)` |
| `kbResourceGetPosition` | `vector kbResourceGetPosition (int resourceID)` | `vector kbResourceGetPosition (int kbResourceID)` |
| `kbResourceGetSubType` | `int kbResourceGetSubType (int resourceID)` | `int kbResourceGetSubType (int kbResourceID)` |
| `kbResourceGetTotalResources` | `float kbResourceGetTotalResources (int resourceID)` | `float kbResourceGetTotalResources (int kbResourceID)` |
| `kbResourceGetType` | `int kbResourceGetType (int resourceID)` | `int kbResourceGetType (int kbResourceID)` |
| `kbResourceGetUnit` | `int kbResourceGetUnit (int resourceID, int index)` | `int kbResourceGetUnit (int kbResourceID, int index)` |
| `kbSetResourceSelectorFactor` | `void kbSetResourceSelectorFactor (int type, int resourceType, float val)` | `void kbSetResourceSelectorFactor (int type, int resourceID, float val)` |
| `kbUnitCount` | `int kbUnitCount (int unitTypeID, int playerID, int stateID)` | `int kbUnitCount (int unitTypeID, int playerID, int state, bool excludeKnockedOutUnits)` |
| `kbUnitGetStatString` | `string kbUnitGetStatString (int unitID, int stat)` | `string kbUnitGetStatString (int unitID, int statEnumID)` |
| `kbUnitIsEmpowered` | `bool kbUnitIsEmpowered (int uID)` | `bool kbUnitIsEmpowered (int unitID)` |
| `kbUnitPickSetPreferenceFactor` | `bool kbUnitPickSetPreferenceFactor (int upID, int unitTypeID, float baseFactor)` | `bool kbUnitPickSetPreferenceFactor (int upID, int unitTypeID, float preferenceFactor)` |
| `kbUnitQueryGetUnitHitpoints` | `float kbUnitQueryGetUnitHitpoints (int queryID, bool currentHitpoints)` | `float kbUnitQueryGetUnitHitpoints (int queryID, bool considerHealth)` |
| `kbUnitQuerySetPlayerRelation` | `void kbUnitQuerySetPlayerRelation (int queryID, int relation)` | `void kbUnitQuerySetPlayerRelation (int queryID, int relation, bool resetQueryData)` |
| `kbUnitQuerySetState` | `void kbUnitQuerySetState (int queryID, int unitState)` | `void kbUnitQuerySetState (int queryID, int v)` |
| `kbUnitTypeCount` | `int kbUnitTypeCount (string unitTypeName, int playerID, int stateID, bool excludeKnockout)` | `int kbUnitTypeCount (string unitTypeName, int player, int stateID, bool excludeKnockedoutUnits)` |
| `kbUnitTypeCountInArea` | `int kbUnitTypeCountInArea (string unitTypeName, int playerID, int stateID, int centerUnitID, float radius)` | `int kbUnitTypeCountInArea (string unitTypeName, int player, int stateID, int centerUnitID, float radius)` |
| `log` | `float log (float _X)` | `float log (float x)` |
| `log10` | `float log10 (float _X)` | `float log10 (float x)` |
| `log2` | `float log2 (float _X)` | `float log2 (float x)` |
| `max` | `float max (float _X, float _Y)` | `float max (float a, float b)` |
| `min` | `float min (float _X, float _Y)` | `float min (float a, float b)` |
| `pow` | `float pow (float _X, float _Y)` | `float pow (float x, float y)` |
| `rmAddClosestLocConstraint` | `bool rmAddClosestLocConstraint (int constraintID)` | `bool rmAddClosestLocConstraint (int constraintID, float bufferDist)` |
| `rmAddGlobalHeightNoise` | `bool rmAddGlobalHeightNoise (int type, float amplitude, float baseFrequency, int numOctaves, float persistence)` | `bool rmAddGlobalHeightNoise (int noiseType, float amplitude, float baseFrequency, int numOctaves, float persistence)` |
| `rmAreaAddHeightConstraint` | `bool rmAreaAddHeightConstraint (int areaID, int constraintID, float minBufferDist, float maxBufferDist)` | `bool rmAreaAddHeightConstraint (int areaDefID, int constraintID, float bufferDist)` |
| `rmAreaAddOriginConstraint` | `bool rmAreaAddOriginConstraint (int areaID, int constraintID, float minBufferDist, float maxBufferDist)` | `bool rmAreaAddOriginConstraint (int areaID, int constraintID, float bufferDist)` |
| `rmAreaBuild` | `bool rmAreaBuild (int areaID, bool doPaint)` | `bool rmAreaBuild (int areaID, bool doPaint, bool warnIfBuilt)` |
| `rmAreaBuildMany` | `void rmAreaBuildMany (int[] areaIDs, bool doPaint, bool buildConcurrently)` | `int rmAreaBuildMany (int[] areaIDs, bool doPaint, bool buildConcurrently, bool warnIfBuilt)` |
| `rmAreaDefAddCliffEdgeConstraint` | `bool rmAreaDefAddCliffEdgeConstraint (int areaID, int typeID, int constraintID, float bufferDist)` | `bool rmAreaDefAddCliffEdgeConstraint (int areaDefID, int typeID, int constraintID, float bufferDist)` |
| `rmAreaDefAddCliffOuterLayerConstraint` | `bool rmAreaDefAddCliffOuterLayerConstraint (int areaID, int constraintID, float bufferDist)` | `bool rmAreaDefAddCliffOuterLayerConstraint (int areaDefID, int constraintID, float bufferDist)` |
| `rmAreaDefAddCliffRampAtAngle` | `bool rmAreaDefAddCliffRampAtAngle (int areaID, float fraction, float angle)` | `bool rmAreaDefAddCliffRampAtAngle (int areaDefID, float fraction, float angle)` |
| `rmAreaDefAddConstraint` | `bool rmAreaDefAddConstraint (int areaID, int constraintID, float minBufferDist, float maxBufferDist)` | `bool rmAreaDefAddConstraint (int areaDefID, int constraintID, float minBufferDist, float maxBufferDist)` |
| `rmAreaDefAddHeightBlend` | `int rmAreaDefAddHeightBlend (int areaID, int blendType, int filterID, int expansionTiles, int numPasses, bool incrementalExpansion, bool blendAfterPaint)` | `int rmAreaDefAddHeightBlend (int areaID, int blendType, int filterID, int expansionTiles, int numPasses, bool incrementalExpansion, bool blendBeforePaint)` |
| `rmAreaDefAddHeightConstraint` | `bool rmAreaDefAddHeightConstraint (int areaID, int constraintID, float minBufferDist, float maxBufferDist)` | `bool rmAreaDefAddHeightConstraint (int areaDefID, int constraintID, float bufferDist)` |
| `rmAreaDefAddInfluencePoint` | `bool rmAreaDefAddInfluencePoint (int areaID, vector loc)` | `bool rmAreaDefAddInfluencePoint (int areaDefID, vector loc)` |
| `rmAreaDefAddInfluenceSegment` | `bool rmAreaDefAddInfluenceSegment (int areaID, vector startLoc, vector endLoc)` | `bool rmAreaDefAddInfluenceSegment (int areaDefID, vector startLoc, vector endLoc)` |
| `rmAreaDefAddOriginConstraint` | `bool rmAreaDefAddOriginConstraint (int areaID, int constraintID, float minBufferDist, float maxBufferDist)` | `bool rmAreaDefAddOriginConstraint (int areaDefID, int constraintID, float bufferDist)` |
| `rmAreaDefAddRemoveType` | `bool rmAreaDefAddRemoveType (int areaID, int typeID)` | `bool rmAreaDefAddRemoveType (int areaDefID, int typeID)` |
| `rmAreaDefAddTerrainLayer` | `bool rmAreaDefAddTerrainLayer (int areaID, int terrainID, int minTileDistance, int maxTileDistance)` | `bool rmAreaDefAddTerrainLayer (int areaDefID, int terrainID, int minTileDistance, int maxTileDistance)` |
| `rmAreaDefAddTerrainMixLayer` | `bool rmAreaDefAddTerrainMixLayer (int areaID, int mixID, int minTileDistance, int maxTileDistance)` | `bool rmAreaDefAddTerrainMixLayer (int areaDefID, int mixID, int minTileDistance, int maxTileDistance)` |
| `rmAreaDefAddTerrainReplacement` | `bool rmAreaDefAddTerrainReplacement (int areaID, int terrainID, int newTerrainID)` | `bool rmAreaDefAddTerrainReplacement (int areaDefID, int terrainID, int newTerrainID)` |
| `rmAreaDefAddToClass` | `bool rmAreaDefAddToClass (int areaID, int classID)` | `bool rmAreaDefAddToClass (int areaDefID, int classID)` |
| `rmAreaDefGetCreatedArea` | `int rmAreaDefGetCreatedArea (int areaDefID, int idx)` | `int rmAreaDefGetCreatedArea (int areaDefID, int index)` |
| `rmAreaDefSetAvoidSelfDistance` | `bool rmAreaDefSetAvoidSelfDistance (int areaDefID, float distance)` | `bool rmAreaDefSetAvoidSelfDistance (int areaDefID, float distance, float bufferDistance)` |
| `rmAreaDefSetBlobDistance` | `bool rmAreaDefSetBlobDistance (int areaID, float minDist, float maxDist)` | `bool rmAreaDefSetBlobDistance (int areaDefID, float minDist, float maxDist)` |
| `rmAreaDefSetBlobs` | `bool rmAreaDefSetBlobs (int areaID, int minBlobs, int maxBlobs)` | `bool rmAreaDefSetBlobs (int areaDefID, int minBlobs, int maxBlobs)` |
| `rmAreaDefSetCliffEmbellishmentDensity` | `bool rmAreaDefSetCliffEmbellishmentDensity (int areaID, float density)` | `bool rmAreaDefSetCliffEmbellishmentDensity (int areaDefID, float density)` |
| `rmAreaDefSetCliffLayerEmbellishmentDensity` | `bool rmAreaDefSetCliffLayerEmbellishmentDensity (int areaID, int layer, float density)` | `bool rmAreaDefSetCliffLayerEmbellishmentDensity (int areaDefID, int layer, float density)` |
| `rmAreaDefSetCliffLayerPaint` | `bool rmAreaDefSetCliffLayerPaint (int areaID, int layer, bool doPaint)` | `bool rmAreaDefSetCliffLayerPaint (int areaDefID, int layer, bool doPaint)` |
| `rmAreaDefSetCliffPaintInsideAsSide` | `bool rmAreaDefSetCliffPaintInsideAsSide (int areaID, bool paintTopAsSide)` | `bool rmAreaDefSetCliffPaintInsideAsSide (int areaDefID, bool paintTopAsSide)` |
| `rmAreaDefSetCliffRampSteepness` | `bool rmAreaDefSetCliffRampSteepness (int areaID, float rampSteepness)` | `bool rmAreaDefSetCliffRampSteepness (int areaDefID, float rampSteepness)` |
| `rmAreaDefSetCliffRamps` | `bool rmAreaDefSetCliffRamps (int areaID, int count, float size, float variance, float spacing, float angle)` | `bool rmAreaDefSetCliffRamps (int areaDefID, int count, float size, float variance, float spacing, float angle)` |
| `rmAreaDefSetCliffSideRadius` | `bool rmAreaDefSetCliffSideRadius (int areaID, int innerRadius, int outerRadius)` | `bool rmAreaDefSetCliffSideRadius (int areaDefID, int innerRadius, int outerRadius)` |
| `rmAreaDefSetCliffSideSheernessThreshold` | `bool rmAreaDefSetCliffSideSheernessThreshold (int areaID, float sheernessAngleThresh)` | `bool rmAreaDefSetCliffSideSheernessThreshold (int areaDefID, float sheernessAngleThresh)` |
| `rmAreaDefSetCliffType` | `bool rmAreaDefSetCliffType (int areaID, int cliffID)` | `bool rmAreaDefSetCliffType (int areaDefID, int cliffID)` |
| `rmAreaDefSetCoherence` | `bool rmAreaDefSetCoherence (int areaID, float coherence, float minDistThresh)` | `bool rmAreaDefSetCoherence (int areaDefID, float coherence, float minDistThresh)` |
| `rmAreaDefSetConstraintBuffer` | `bool rmAreaDefSetConstraintBuffer (int areaID, float minBufferDist, float maxBufferDist)` | `bool rmAreaDefSetConstraintBuffer (int areaDefID, float minBufferDist, float maxBufferDist)` |
| `rmAreaDefSetEdgeSmoothDistance` | `bool rmAreaDefSetEdgeSmoothDistance (int areaID, int smoothDistance, bool smoothOnMapEdge)` | `bool rmAreaDefSetEdgeSmoothDistance (int areaDefID, int smoothDistance, bool smoothOnMapEdge)` |
| `rmAreaDefSetForestTreeDensity` | `bool rmAreaDefSetForestTreeDensity (int areaID, float density)` | `bool rmAreaDefSetForestTreeDensity (int areaDefID, float density)` |
| `rmAreaDefSetForestType` | `bool rmAreaDefSetForestType (int areaID, int forestID)` | `bool rmAreaDefSetForestType (int areaDefID, int forestID)` |
| `rmAreaDefSetForestUnderbrushDensity` | `bool rmAreaDefSetForestUnderbrushDensity (int areaID, float density)` | `bool rmAreaDefSetForestUnderbrushDensity (int areaDefID, float frequency)` |
| `rmAreaDefSetHeight` | `bool rmAreaDefSetHeight (int areaID, float height)` | `bool rmAreaDefSetHeight (int areaDefID, float height)` |
| `rmAreaDefSetHeightFactors` | `bool rmAreaDefSetHeightFactors (int areaID, float oneTileFactor, float twoTilesFactor, float threeTilesFactor, float fourTilesFactor)` | `bool rmAreaDefSetHeightFactors (int areaDefID, float oneTileFactor, float twoTilesFactor, float threeTilesFactor, float fourTilesFactor)` |
| `rmAreaDefSetHeightNoiseBias` | `bool rmAreaDefSetHeightNoiseBias (int areaID, float bias)` | `bool rmAreaDefSetHeightNoiseBias (int areaDefID, float bias)` |
| `rmAreaDefSetHeightNoiseEdgeFalloffDist` | `bool rmAreaDefSetHeightNoiseEdgeFalloffDist (int areaID, float dist)` | `bool rmAreaDefSetHeightNoiseEdgeFalloffDist (int areaDefID, float dist)` |
| `rmAreaDefSetHeightRelative` | `bool rmAreaDefSetHeightRelative (int areaID, float height)` | `bool rmAreaDefSetHeightRelative (int areaDefID, float height)` |
| `rmAreaDefSetLoc` | `bool rmAreaDefSetLoc (int areaID, vector loc)` | `bool rmAreaDefSetLoc (int areaDefID, vector loc)` |
| `rmAreaDefSetLocPlayer` | `bool rmAreaDefSetLocPlayer (int areaID, int playerID)` | `bool rmAreaDefSetLocPlayer (int areaDefID, int playerID, int playerLocIndex)` |
| `rmAreaDefSetLocTeam` | `bool rmAreaDefSetLocTeam (int areaID, int teamID)` | `bool rmAreaDefSetLocTeam (int areaDefID, int teamID)` |
| `rmAreaDefSetMix` | `bool rmAreaDefSetMix (int areaID, int mixID)` | `bool rmAreaDefSetMix (int areaDefID, int mixID)` |
| `rmAreaDefSetOriginConstraintBuffer` | `bool rmAreaDefSetOriginConstraintBuffer (int areaID, float minBufferDist, float maxBufferDist)` | `bool rmAreaDefSetOriginConstraintBuffer (int areaDefID, float bufferDist)` |
| `rmAreaDefSetParent` | `bool rmAreaDefSetParent (int areaID, int parentAreaID)` | `bool rmAreaDefSetParent (int areaDefID, int parentAreaID)` |
| `rmAreaDefSetPath` | `bool rmAreaDefSetPath (int areaID, int pathID, float minWidthMeters, float extraWidthMeters)` | `bool rmAreaDefSetPath (int areaDefID, int pathID, float minWidthMeters, float extraWidthMeters)` |
| `rmAreaDefSetPathSegment` | `bool rmAreaDefSetPathSegment (int areaID, int pathID, int segmentIdx, float minWidthMeters, float extraWidthMeters)` | `bool rmAreaDefSetPathSegment (int areaDefID, int pathID, int segmentIdx, float minWidthMeters, float extraWidthMeters)` |
| `rmAreaDefSetReveal` | `bool rmAreaDefSetReveal (int areaID, int tiles)` | `bool rmAreaDefSetReveal (int areaDefID, int tiles)` |
| `rmAreaDefSetSize` | `bool rmAreaDefSetSize (int areaID, float fraction, float minSuccessFraction)` | `bool rmAreaDefSetSize (int areaDefID, float fraction, float minSuccessFraction)` |
| `rmAreaDefSetSizeRange` | `bool rmAreaDefSetSizeRange (int areaID, float minFraction, float maxFraction, float minSuccessFraction)` | `bool rmAreaDefSetSizeRange (int areaDefID, float minFraction, float maxFraction, float minSuccessFraction)` |
| `rmAreaDefSetTerrainType` | `bool rmAreaDefSetTerrainType (int areaID, int terrainID)` | `bool rmAreaDefSetTerrainType (int areaDefID, int terrainID)` |
| `rmAreaDefSetWarnOnBuildFailure` | `bool rmAreaDefSetWarnOnBuildFailure (int areaID, int minAcceptedState)` | `bool rmAreaDefSetWarnOnBuildFailure (int areaDefID, int minAcceptedState)` |
| `rmAreaDefSetWaterDepth` | `bool rmAreaDefSetWaterDepth (int areaID, float depth)` | `bool rmAreaDefSetWaterDepth (int areaDefID, float depth)` |
| `rmAreaDefSetWaterEdgeHeight` | `bool rmAreaDefSetWaterEdgeHeight (int areaID, float height, float bufferDistance)` | `bool rmAreaDefSetWaterEdgeHeight (int areaDefID, float height, float bufferDistance)` |
| `rmAreaDefSetWaterHeight` | `bool rmAreaDefSetWaterHeight (int areaID, float height, int heightType)` | `bool rmAreaDefSetWaterHeight (int areaDefID, float height, int heightType)` |
| `rmAreaDefSetWaterHeightBlend` | `bool rmAreaDefSetWaterHeightBlend (int areaID, int filterID, float smoothDistance, int numPasses)` | `bool rmAreaDefSetWaterHeightBlend (int areaDefID, int filterID, float smoothDistance, int numPasses)` |
| `rmAreaDefSetWaterType` | `bool rmAreaDefSetWaterType (int areaID, int waterID)` | `bool rmAreaDefSetWaterType (int areaDefID, int waterID)` |
| `rmAreaGetClosestLoc` | `vector rmAreaGetClosestLoc (int areaID, vector loc, int constraintID)` | `vector rmAreaGetClosestLoc (int areaID, vector loc, int[] constraintIDs)` |
| `rmAreaPaint` | `bool rmAreaPaint (int areaID)` | `bool rmAreaPaint (int areaID, bool warnOnError)` |
| `rmAreaPaintMany` | `void rmAreaPaintMany (int[] areaIDs)` | `int rmAreaPaintMany (int[] areaIDs, bool warnOnError)` |
| `rmAreaSetForestUnderbrushDensity` | `bool rmAreaSetForestUnderbrushDensity (int areaID, float density)` | `bool rmAreaSetForestUnderbrushDensity (int areaID, float frequency)` |
| `rmAreaSetLocPlayer` | `bool rmAreaSetLocPlayer (int areaID, int playerID)` | `bool rmAreaSetLocPlayer (int areaID, int playerID, int playerLocIndex)` |
| `rmAreaSetOriginConstraintBuffer` | `bool rmAreaSetOriginConstraintBuffer (int areaID, float minBufferDist, float maxBufferDist)` | `bool rmAreaSetOriginConstraintBuffer (int areaID, float bufferDist)` |
| `rmAreaSetSize` | `bool rmAreaSetSize (int areaID, float fraction, float minSuccessFraction)` | `bool rmAreaSetSize (int areaID, float minFraction, float minSuccessFraction)` |
| `rmCreateCircularConstraint` | `int rmCreateCircularConstraint (vector loc, float radiusMeters, float minAngle, float maxAngle, string name)` | `int rmCreateCircularConstraint (vector loc, float radiusMeters, float minAngle, float maxAngle, bool inverted, string name)` |
| `rmCreateMaxHeightConstraint` | `int rmCreateMaxHeightConstraint (float maxHeight, string name)` | `int rmCreateMaxHeightConstraint (float height, string name)` |
| `rmCreateMaxWaterDepthConstraint` | `int rmCreateMaxWaterDepthConstraint (float maxWaterDepth, string name)` | `int rmCreateMaxWaterDepthConstraint (float depth, string name)` |
| `rmCreateMinHeightConstraint` | `int rmCreateMinHeightConstraint (float minHeight, string name)` | `int rmCreateMinHeightConstraint (float height, string name)` |
| `rmCreateMinWaterDepthConstraint` | `int rmCreateMinWaterDepthConstraint (float minWaterDepth, string name)` | `int rmCreateMinWaterDepthConstraint (float depth, string name)` |
| `rmCreateTileDistanceConstraint` | `int rmCreateTileDistanceConstraint (int tileX, int tileZ, float minDist, string name)` | `int rmCreateTileDistanceConstraint (vector tile, float minDist, string name)` |
| `rmCreateTileMaxDistanceConstraint` | `int rmCreateTileMaxDistanceConstraint (int tileX, int tileZ, float maxDist, string name)` | `int rmCreateTileMaxDistanceConstraint (vector tile, float maxDist, string name)` |
| `rmCustomForestSetTerrain` | `bool rmCustomForestSetTerrain (int forestID, int terrainID)` | `bool rmCustomForestSetTerrain (int forestID, int terrainTypeID)` |
| `rmEchoError` | `void rmEchoError (string text)` | `void rmEchoError (string errorString)` |
| `rmEchoInfo` | `void rmEchoInfo (string text)` | `void rmEchoInfo (string echoString)` |
| `rmEchoWarning` | `void rmEchoWarning (string text)` | `void rmEchoWarning (string warningString)` |
| `rmFractionToMeters` | `vector rmFractionToMeters (vector fraction, bool clamp, bool warn)` | `vector rmFractionToMeters (vector meters, bool clamp, bool warn)` |
| `rmFractionToTileIndex` | `vector rmFractionToTileIndex (vector fraction, bool warn)` | `vector rmFractionToTileIndex (vector fraction, bool clamp, bool warn)` |
| `rmGenerationSetSuccess` | `void rmGenerationSetSuccess (bool status)` | `void rmGenerationSetSuccess (bool success)` |
| `rmGetPlayerLoc` | `vector rmGetPlayerLoc (int playerID)` | `vector rmGetPlayerLoc (int playerID, int locIdx)` |
| `rmInitializeLand` | `bool rmInitializeLand (int terrainID, float baseHeight)` | `bool rmInitializeLand (int terrainID, float height)` |
| `rmInitializeMix` | `bool rmInitializeMix (int mixID, float baseHeight)` | `bool rmInitializeMix (int mixID, float height)` |
| `rmLocGenApply` | `bool rmLocGenApply (bool buildAreas, bool paintAras)` | `bool rmLocGenApply (bool buildAreas, bool paintAreas)` |
| `rmLocGenSetLocAngleVariance` | `bool rmLocGenSetLocAngleVariance (int locID, float angleVar, bool isAbsolute)` | `bool rmLocGenSetLocAngleVariance (int locID, float angleVar, bool useMeters)` |
| `rmLocGenSetLocOwner` | `bool rmLocGenSetLocOwner (int locID, int ownerID)` | `bool rmLocGenSetLocOwner (int locID, int ownerID, int ownerIndex)` |
| `rmMetersToTileIndex` | `vector rmMetersToTileIndex (vector meters, bool warn)` | `vector rmMetersToTileIndex (vector meters, bool clamp, bool warn)` |
| `rmMetersToTiles` | `int rmMetersToTiles (float meters)` | `float rmMetersToTiles (float meters)` |
| `rmObjectAddConstraint` | `bool rmObjectAddConstraint (int objectID, int constraintID, float bufferDist)` | `bool rmObjectAddConstraint (int objectID, int constraintID, int bufferType, float bufferDist)` |
| `rmObjectAddItem` | `bool rmObjectAddItem (int objectID, int puid, int count, float minClusterDist, float maxClusterDist)` | `int rmObjectAddItem (int objectID, int protoID, int count, float minClusterDist, float maxClusterDist)` |
| `rmObjectDefAddConstraint` | `bool rmObjectDefAddConstraint (int objectDefID, int constraintID, float bufferDist)` | `bool rmObjectDefAddConstraint (int objectDefID, int constraintID, int bufferType, float bufferDist)` |
| `rmObjectDefAddItem` | `bool rmObjectDefAddItem (int objectDefID, int puid, int count, float minClusterDist, float maxClusterDist)` | `int rmObjectDefAddItem (int objectDefID, int protoID, int count, float minClusterDist, float maxClusterDist)` |
| `rmObjectDefAddItemRange` | `bool rmObjectDefAddItemRange (int objectDefID, int puid, int minCount, int maxCount, float minClusterDist, float maxClusterDist)` | `int rmObjectDefAddItemRange (int objectDefID, int protoID, int minCount, int maxCount, float minClusterDist, float maxClusterDist)` |
| `rmObjectDefAddToClass` | `bool rmObjectDefAddToClass (int objectID, int classID)` | `bool rmObjectDefAddToClass (int objectDefID, int classID)` |
| `rmObjectDefCreateObject` | `int rmObjectDefCreateObject (int objectDefID, string name)` | `int rmObjectDefCreateObject (int objectDef, string name)` |
| `rmObjectDefGetCreatedObject` | `int rmObjectDefGetCreatedObject (int objectDefID, int idx)` | `int rmObjectDefGetCreatedObject (int objectDefID, int index)` |
| `rmObjectDefGetName` | `string rmObjectDefGetName (int objectDefID)` | `string rmObjectDefGetName (int defID)` |
| `rmObjectDefPlaceAnywhere` | `int[] rmObjectDefPlaceAnywhere (int objectDefID, int playerID, int count, bool ignoreConstraints)` | `int[] rmObjectDefPlaceAnywhere (int objectID, int playerID, int count, bool ignoreConstraints)` |
| `rmObjectDefPlaceAtArea` | `int[] rmObjectDefPlaceAtArea (int objectDefID, int playerID, int areaID, float minDistMeters, float maxDistMeters, int count, bool squareRadius, bool ignoreConstraints)` | `int[] rmObjectDefPlaceAtArea (int objectDefID, int playerID, int areaID, float minDist, float maxDist, int count, bool squareRadius, bool ignoreConstraints)` |
| `rmObjectDefPlaceAtLoc` | `int[] rmObjectDefPlaceAtLoc (int objectDefID, int playerID, vector loc, float minDistMeters, float maxDistMeters, int count, bool squareRadius, bool ignoreConstraints)` | `int[] rmObjectDefPlaceAtLoc (int objectDefID, int playerID, vector loc, float minDist, float maxDist, int count, bool squareRadius, bool ignoreConstraints)` |
| `rmObjectDefSetItemRotation` | `bool rmObjectDefSetItemRotation (int objectDefID, int itemIdx, int rotationType, float rotationAngle)` | `bool rmObjectDefSetItemRotation (int objectDefID, int itemIdex, int rotationType, float rotationAngle)` |
| `rmObjectDefSetItemVariation` | `bool rmObjectDefSetItemVariation (int objectDefID, int itemIdx, int variation)` | `bool rmObjectDefSetItemVariation (int objectDefID, int itemIdex, int variation)` |
| `rmObjectGetName` | `string rmObjectGetName (int objectID)` | `string rmObjectGetName (int defID)` |
| `rmObjectPlaceAtArea` | `bool rmObjectPlaceAtArea (int objectID, int playerID, int areaID, float minDistMeters, float maxDistMeters, bool squareRadius, bool ignoreConstraints)` | `bool rmObjectPlaceAtArea (int objectID, int playerID, int areaID, float minDist, float maxDist, bool squareRadius, bool ignoreConstraints)` |
| `rmObjectPlaceAtLoc` | `bool rmObjectPlaceAtLoc (int objectID, int playerID, vector loc, float minDistMeters, float maxDistMeters, bool squareRadius, bool ignoreConstraints)` | `bool rmObjectPlaceAtLoc (int objectID, int playerID, vector loc, float minDist, float maxDist, bool squareRadius, bool ignoreConstraints)` |
| `rmObjectSetItemRotation` | `bool rmObjectSetItemRotation (int objectID, int itemIdx, int rotationType, float rotationAngle)` | `bool rmObjectSetItemRotation (int objectID, int itemIdex, int rotationType, float rotationAngle)` |
| `rmObjectSetItemVariation` | `bool rmObjectSetItemVariation (int objectID, int itemIdx, int variation)` | `bool rmObjectSetItemVariation (int objectID, int itemIdex, int variation)` |
| `rmPathAddWaypoint` | `int rmPathAddWaypoint (int pathID, vector loc, float originDistMeters)` | `int rmPathAddWaypoint (int pathID, vector loc, float minDistMeters, float maxDistMeters)` |
| `rmPathAddWaypointInArea` | `int rmPathAddWaypointInArea (int pathID, int areaID, float originDistMeters)` | `int rmPathAddWaypointInArea (int pathID, int areaID, float minOriginDistMeters, float maxOriginDistMeters)` |
| `rmPathDefAddToClass` | `bool rmPathDefAddToClass (int pathID, int classID)` | `bool rmPathDefAddToClass (int pathDefID, int classID)` |
| `rmPathDefAddWaypoint` | `int rmPathDefAddWaypoint (int pathDefID, vector loc, float originDistMeters)` | `int rmPathDefAddWaypoint (int pathDefID, vector loc, float minDistMeters, float maxDistMeters)` |
| `rmPathDefAddWaypointInArea` | `int rmPathDefAddWaypointInArea (int pathDefID, int areaID, float originDistMeters)` | `int rmPathDefAddWaypointInArea (int pathDefID, int areaID, float minOriginDistMeters, float maxOriginDistMeters)` |
| `rmPathDefGetCreatedPath` | `int rmPathDefGetCreatedPath (int pathDefID, int idx)` | `int rmPathDefGetCreatedPath (int pathDefID, int index)` |
| `rmPathGetName` | `string rmPathGetName (int pathID)` | `string rmPathGetName (int defID)` |
| `rmPlacePlayer` | `bool rmPlacePlayer (int playerID, vector loc)` | `int rmPlacePlayer (int playerID, vector loc)` |
| `rmPlacePlayersOnCircle` | `bool rmPlacePlayersOnCircle (float radius, float radiusMetersVar, float angleVar, float angle, float range, vector loc)` | `bool rmPlacePlayersOnCircle (float radius, float radiusMetersVar, float angleVar, float angle, float range, vector originLoc)` |
| `rmPlacePlayersOnSquare` | `bool rmPlacePlayersOnSquare (float xRadius, float zRadius, float lineVarMeters, float distVarMeters, vector loc)` | `bool rmPlacePlayersOnSquare (float xRadiusFraction, float zRadiusFraction, float lineVarMeters, float distVarMeters, vector loc)` |
| `rmRemoveUnitType` | `int rmRemoveUnitType (int type)` | `int rmRemoveUnitType (int unitType)` |
| `rmSetMapSize` | `bool rmSetMapSize (int x, int z)` | `bool rmSetMapSize (int xTiles, int zTiles)` |
| `rmSetPlayerResource` | `bool rmSetPlayerResource (int playerID, int resourceID, float amount)` | `bool rmSetPlayerResource (int playerID, int resouceID, float amount)` |
| `rmSetTeamPlayerOrderType` | `bool rmSetTeamPlayerOrderType (int orderType)` | `bool rmSetTeamPlayerOrderType (int type)` |
| `rmSetTeamSpacingModifier` | `bool rmSetTeamSpacingModifier (float modifier)` | `void rmSetTeamSpacingModifier (float modifier)` |
| `rmSplineGetName` | `string rmSplineGetName (int splineID)` | `string rmSplineGetName (int defID)` |
| `rmSplineToPaths` | `int[] rmSplineToPaths (int splineID, int numPointsPerSplineSegment, bool allowDiagonals)` | `int[] rmSplineToPaths (int splineID, int pathDefID, int numPointsPerSplineSegment)` |
| `rmSquareMetersToAreaFraction` | `float rmSquareMetersToAreaFraction (float meters, bool clamp, bool warn)` | `float rmSquareMetersToAreaFraction (float squareMeters, bool clamp, bool warn)` |
| `rmTileIndexToFraction` | `vector rmTileIndexToFraction (vector tile, bool warn)` | `vector rmTileIndexToFraction (vector tile, bool clamp, bool warn)` |
| `rmTileIndexToMeters` | `vector rmTileIndexToMeters (vector tile, bool warn)` | `vector rmTileIndexToMeters (vector tile, bool clamp, bool warn)` |
| `rmTilesToMeters` | `float rmTilesToMeters (int tiles)` | `float rmTilesToMeters (float tiles)` |
| `rmXFractionToMeters` | `float rmXFractionToMeters (float fraction, bool clamp, bool warn)` | `float rmXFractionToMeters (float meters, bool clamp, bool warn)` |
| `rmXFractionToTileIndex` | `int rmXFractionToTileIndex (float fraction, bool warn)` | `int rmXFractionToTileIndex (float fraction, bool clamp, bool warn)` |
| `rmXMetersToTileIndex` | `int rmXMetersToTileIndex (float fraction, bool warn)` | `int rmXMetersToTileIndex (float meters, bool clamp, bool warn)` |
| `rmXTileIndexToFraction` | `float rmXTileIndexToFraction (int tile, bool warn)` | `float rmXTileIndexToFraction (int tile, bool clamp, bool warn)` |
| `rmXTileIndexToMeters` | `float rmXTileIndexToMeters (int tile, bool warn)` | `float rmXTileIndexToMeters (int tile, bool clamp, bool warn)` |
| `rmZFractionToMeters` | `float rmZFractionToMeters (float fraction, bool clamp, bool warn)` | `float rmZFractionToMeters (float meters, bool clamp, bool warn)` |
| `rmZFractionToTileIndex` | `int rmZFractionToTileIndex (float fraction, bool warn)` | `int rmZFractionToTileIndex (float fraction, bool clamp, bool warn)` |
| `rmZMetersToTileIndex` | `int rmZMetersToTileIndex (float fraction, bool warn)` | `int rmZMetersToTileIndex (float meters, bool clamp, bool warn)` |
| `rmZTileIndexToFraction` | `float rmZTileIndexToFraction (int tile, bool warn)` | `float rmZTileIndexToFraction (int tile, bool clamp, bool warn)` |
| `rmZTileIndexToMeters` | `float rmZTileIndexToMeters (int tile, bool warn)` | `float rmZTileIndexToMeters (int tile, bool clamp, bool warn)` |
| `round` | `float round (float _X)` | `float round (float x)` |
| `sin` | `float sin (float _X)` | `float sin (float x)` |
| `sqrt` | `float sqrt (float _X)` | `float sqrt (float x)` |
| `tan` | `float tan (float _X)` | `float tan (float x)` |
| `trAISetAttackResponseDistance` | `void trAISetAttackResponseDistance (int playerID, float AttackResponseDistance)` | `void trAISetAttackResponseDistance (int playerID, float attackResponseDistance)` |
| `trBuildingTimeShiftAtPos` | `bool trBuildingTimeShiftAtPos (int unitID, float posX, float posY, float posZ)` | `bool trBuildingTimeShiftAtPos (int unitID, float x, float y, float z)` |
| `trChatHistoryContains` | `bool trChatHistoryContains (string text, int player)` | `bool trChatHistoryContains (string text, int playerID)` |
| `trCounterAddGenericXS` | `void trCounterAddGenericXS (string name, string msg, string appendMsg, string xsCall, int eventID, int initialVal, int finalVal, bool finalAsMin, bool showFinal, bool reverseCount, bool startAtZero)` | `void trCounterAddGenericXS (string name, string msg, string appendMsg, string xsCall, int eventID, int intialVal, int finalVal, bool finalAsMin, bool showFinal, bool reverseCount, bool startAtZero)` |
| `trCounterSetManual` | `bool trCounterSetManual (string name, int value)` | `bool trCounterSetManual (string name, int val)` |
| `trDamageUnitsPercentInArea` | `void trDamageUnitsPercentInArea (int playerID, string unitTypeName, float range, float dmgPercent)` | `void trDamageUnitsPercentInArea (int playerID, string unitTypeName, float range, float healPercent)` |
| `trEchoStatValue` | `void trEchoStatValue (int playerID, int statTypeID)` | `void trEchoStatValue (int playerID, int statIndex)` |
| `trFakifySelectionSubModelByOverrideName` | `void trFakifySelectionSubModelByOverrideName (string submodelOverrideName, int fakePlayerIndex)` | `void trFakifySelectionSubModelByOverrideName (string overrideName, int fakePlayerIndex)` |
| `trGetTerrainHeight` | `float trGetTerrainHeight (vector center)` | `float trGetTerrainHeight (vector position)` |
| `trGetTerrainSubtype` | `int trGetTerrainSubtype (vector center)` | `int trGetTerrainSubtype (vector position)` |
| `trGetTerrainType` | `int trGetTerrainType (vector center)` | `int trGetTerrainType (vector position)` |
| `trGetWaterType` | `int trGetWaterType (vector center)` | `int trGetWaterType (vector position)` |
| `trGodPowerEnableBlocking` | `void trGodPowerEnableBlocking (bool enable)` | `void trGodPowerEnableBlocking (bool bEnable)` |
| `trGodPowerSetCost` | `void trGodPowerSetCost (int playerID, string protoPowerName, float cost, float repeatCost)` | `void trGodPowerSetCost (int playerID, string protoPowerName, float initialCost, float repeatCost)` |
| `trGodPowerSetUsedTimes` | `void trGodPowerSetUsedTimes (int playerID, string protoPowerName, int numUsedTimes)` | `void trGodPowerSetUsedTimes (int playerID, string protoPowerName, int numUses)` |
| `trModifyProtounitAction` | `void trModifyProtounitAction (string unitTypeName, string protoUnitActionName, int playerID, int puField, float delta, int puRelativity)` | `void trModifyProtounitAction (string unitTypeName, string protoUnitActionName, int playerID, int puField, float delta, int relativity)` |
| `trModifyProtounitActionUnitType` | `void trModifyProtounitActionUnitType (string unitTypeName, string actionName, string unitType, int playerID, int puField, float delta, int puRelativity)` | `void trModifyProtounitActionUnitType (string unitTypeName, string actionName, string unitType, int playerID, int puField, float delta, int relativity)` |
| `trModifyProtounitData` | `void trModifyProtounitData (string unitTypeName, int playerID, int puField, float delta, int puRelativity)` | `void trModifyProtounitData (string unitTypeName, int playerID, int puField, float delta, int relativity)` |
| `trModifyProtounitResource` | `void trModifyProtounitResource (string unitTypeName, string resource, int playerID, int puField, float delta, int puRelativity)` | `void trModifyProtounitResource (string unitTypeName, string resource, int playerID, int puField, float delta, int relativity)` |
| `trMusicSetMood` | `void trMusicSetMood (int moodID)` | `void trMusicSetMood (int moodID, float fadeTimeSeconds)` |
| `trOverlayText` | `void trOverlayText (string rawText, float time, float textSize, int r, int g, int b)` | `void trOverlayText (string rawText, float time, float textSize, int colorR, int colorG, int colorB)` |
| `trPaintTerrainBySubtypeName` | `void trPaintTerrainBySubtypeName (string subTypeName, float x0, float z0, float x1, float z1, bool updateObstructions)` | `void trPaintTerrainBySubtypeName (string subtypeName, float x0, float z0, float x1, float z1, bool updateObstructions)` |
| `trPaintTerrainCircularBySubtypeName` | `void trPaintTerrainCircularBySubtypeName (string subTypeName, vector center, float radius, bool updateObstructions)` | `void trPaintTerrainCircularBySubtypeName (string subtypeName, vector center, float radius, bool updateObstructions)` |
| `trPlaceFoundation` | `int trPlaceFoundation (string protoName, float x, float y, float z, int heading, int playerID)` | `int trPlaceFoundation (string protoName, float x, float y, float z, int heading, int playerID, float pctComplete)` |
| `trPlayerModifyData` | `void trPlayerModifyData (int playerID, int dataField, int attribute, float delta, int puRelativity)` | `void trPlayerModifyData (int playerID, int dataField, int attribute, float delta, int relativity)` |
| `trPlayerModifyResourceData` | `void trPlayerModifyResourceData (int playerID, int dataField, int resourceID, float delta, int puRelativity)` | `void trPlayerModifyResourceData (int playerID, int dataField, int resourceID, float delta, int relativity)` |
| `trPlayerOverrideCivName` | `void trPlayerOverrideCivName (int playerID, string name)` | `void trPlayerOverrideCivName (int playerID, string stringID)` |
| `trProtoUnitChangeName` | `void trProtoUnitChangeName (string protoUnitName, int playerID, string nameStr, string rolloverStr, string shortRolloverStr)` | `void trProtoUnitChangeName (string protoUnitName, int playerID, string nameStrId, string rolloverStrId, string shortRolloverStrId)` |
| `trProtoUnitSetFlag` | `void trProtoUnitSetFlag (int playerID, string unitTypeName, string protoFlagName, bool set)` | `void trProtoUnitSetFlag (int playerID, string srcUnitTypeName, string unitTypeName, bool set)` |
| `trProtounitActionSpecialEffect` | `void trProtounitActionSpecialEffect (string unitTypeName, string protoUnitActionName, int playerID, int effectTypeID, string targetType, int dmgType, float duration, float value)` | `void trProtounitActionSpecialEffect (string unitTypeName, string actionName, int playerID, int effectField, string targetType, int dmgType, float duration, float value)` |
| `trProtounitActionSpecialEffectActive` | `void trProtounitActionSpecialEffectActive (string unitTypeName, string protoUnitActionName, int playerID, int effectTypeID, string targetType, int dmgType, bool active)` | `void trProtounitActionSpecialEffectActive (string unitTypeName, string actionName, int playerID, int effectField, string targetType, int dmgType, bool active)` |
| `trProtounitActionSpecialEffectDuration` | `void trProtounitActionSpecialEffectDuration (string unitTypeName, string protoUnitActionName, int playerID, int effectTypeID, string targetType, int dmgType, float delta, int puRelativity)` | `void trProtounitActionSpecialEffectDuration (string unitTypeName, string protoUnitActionName, int playerID, int efectType, string targetType, int damageType, float delta, int relativity)` |
| `trProtounitActionSpecialEffectModifier` | `void trProtounitActionSpecialEffectModifier (string unitTypeName, string protoUnitActionName, int playerID, int effectTypeID, string targetType, float value, int modifyType, int dmgType)` | `void trProtounitActionSpecialEffectModifier (string unitTypeName, string actionName, int playerID, int effectField, string targetType, float value, int modifyType, int dmgType)` |
| `trProtounitActionSpecialEffectProtoUnit` | `void trProtounitActionSpecialEffectProtoUnit (string unitTypeName, string protoUnitActionName, int playerID, int effectTypeID, string targetType, string protoUnit, float duration, float value)` | `void trProtounitActionSpecialEffectProtoUnit (string unitTypeName, string actionName, int playerID, int effectField, string targetType, string protoUnit, float duration, float value)` |
| `trRelicCreate` | `bool trRelicCreate (float x, float y, float z, int heading, string relicName)` | `bool trRelicCreate (float x, float y, float z, int heading, string relicname)` |
| `trRelicForce` | `bool trRelicForce (int unitID, string relicName)` | `bool trRelicForce (int unitID, string relicname)` |
| `trShowImageDialog` | `void trShowImageDialog (string imagePath, string message)` | `void trShowImageDialog (string imagePath, string subtitle)` |
| `trSoundPlayDialogue` | `void trSoundPlayDialogue (int playerID, string msgStrID, string speakerStrID, string portraitStrID, string sound, int eventID, bool ignoreOnAbort, int timeoutMs)` | `void trSoundPlayDialogue (int playerID, string msgStrID, string speakerStrID, string portraitStrID, string sound, int eventID, bool ignoreOnAbort, int timeoutMs, bool overrideSoundLength)` |
| `trTechHideEffects` | `void trTechHideEffects (int techID, int playerID, bool hide)` | `void trTechHideEffects (int techID, int playerID, bool display)` |
| `trTerrainAtPosition` | `bool trTerrainAtPosition (string subTypeName, vector center)` | `bool trTerrainAtPosition (string subTypeName, vector position)` |
| `trUIResourceEntryFlash` | `void trUIResourceEntryFlash (int buttonIndex, bool flash)` | `void trUIResourceEntryFlash (int entryIndex, bool flash)` |
| `trUnitAdjustModifier` | `void trUnitAdjustModifier (int modifyType, int dmgType, float delta, int relativityIdx)` | `void trUnitAdjustModifier (int modifyType, int dmgType, float delta, int relativity)` |
| `trUnitDistanceToUnitID` | `float trUnitDistanceToUnitID (int unitID)` | `float trUnitDistanceToUnitID (int blockID)` |
| `trUnitModifyResourceInventory` | `void trUnitModifyResourceInventory (int resourceID, float delta, int puRelativity)` | `void trUnitModifyResourceInventory (int resourceID, float delta, int relativity)` |
| `trUnitReposition` | `bool trUnitReposition (float x, float y, float z, bool disableTie, bool immediate)` | `bool trUnitReposition (float x, float y, float z, bool disableTying, bool immediate)` |
| `trUnitRepositionToUnit` | `bool trUnitRepositionToUnit (int unitID, bool disableTie, bool immediate)` | `bool trUnitRepositionToUnit (int unitID, bool disableTying, bool immediate)` |
| `trUnitSetGatherPointPosForPlayer` | `void trUnitSetGatherPointPosForPlayer (int playerID, int unitID, float xpos, float ypos, float zpos)` | `void trUnitSetGatherPointPosForPlayer (int playerID, int sourceID, float x, float y, float z)` |
| `trUnitSetOrientationForward` | `bool trUnitSetOrientationForward (int degrees, bool disableTie)` | `bool trUnitSetOrientationForward (int degrees, bool disableTying)` |
| `trUnitSetOrientationRight` | `bool trUnitSetOrientationRight (int degrees, bool disableTie)` | `bool trUnitSetOrientationRight (int degrees, bool disableTying)` |
| `trUnitSetOrientationUp` | `bool trUnitSetOrientationUp (int degrees, bool disableTie)` | `bool trUnitSetOrientationUp (int degrees, bool disableTying)` |
| `trUnitSetScale` | `void trUnitSetScale (float scaleX, float scaleY, float scaleZ)` | `void trUnitSetScale (float x, float y, float z)` |
| `trUnitSetTactic` | `bool trUnitSetTactic (string tacticName)` | `void trUnitSetTactic (int tacticDBID)` |
| `trUnitSetVeterancyRank` | `void trUnitSetVeterancyRank (int rankID)` | `void trUnitSetVeterancyRank (int rank)` |
| `trWPFDialogOpen` | `bool trWPFDialogOpen (int wpfDialogID)` | `bool trWPFDialogOpen (int wpdDialogID)` |
| `trWaterAtPosition` | `bool trWaterAtPosition (string waterName, vector center)` | `bool trWaterAtPosition (string waterTypeName, vector position)` |
| `trWorldSpacePrompt` | `void trWorldSpacePrompt (string id, int unitID, bool showColor, string text, vector offset, string attachPoint)` | `void trWorldSpacePrompt (string id, int unitID, bool showColor, string stringID, vector offset, string attachPoint, bool showBackground)` |
| `trWorldSpacePromptArea` | `void trWorldSpacePromptArea (string id, vector location, string text, vector offset)` | `void trWorldSpacePromptArea (string id, vector location, string stringID, vector offset, bool showBackground)` |
| `trWorldSpacePromptArmy` | `void trWorldSpacePromptArmy (string id, string armyName, bool showColor, string text, vector offset)` | `void trWorldSpacePromptArmy (string id, string armyName, bool showColor, string stringID, vector offset, bool showBackground)` |
| `xsStringCharAt` | `string xsStringCharAt (string s, int idx)` | `string xsStringCharAt (string s, int index)` |
| `xsStringContains` | `bool xsStringContains (string first, string second, bool caseSensitive)` | `bool xsStringContains (string s, string sub, bool caseSensitive)` |
| `xsStringEndsWith` | `bool xsStringEndsWith (string first, string second, bool caseSensitive)` | `bool xsStringEndsWith (string s, string sub, bool caseSensitive)` |
| `xsStringFindFirst` | `int xsStringFindFirst (string first, string second, int startIdx, bool caseSensitive)` | `int xsStringFindFirst (string s, string sub, int startIdx, bool caseSensitive)` |
| `xsStringFindLast` | `int xsStringFindLast (string first, string second, int startIdx, bool caseSensitive)` | `int xsStringFindLast (string s, string sub, int startIdx, bool caseSensitive)` |
| `xsStringStartsWith` | `bool xsStringStartsWith (string first, string second, bool caseSensitive)` | `bool xsStringStartsWith (string s, string sub, bool caseSensitive)` |
| `xsVectorDistanceToLine` | `float xsVectorDistanceToLine (vector v, vector p, vector dir)` | `float xsVectorDistanceToLine (vector v, vector pointOnLine, vector dir)` |
| `cAttackPlanAttackAnchorPoint` | `const int cAttackPlanAttackAnchorPoint = 26` | `const int cAttackPlanAttackAnchorPoint = 24` |
| `cAttackPlanDoneMode` | `const int cAttackPlanDoneMode = 20` | `const int cAttackPlanDoneMode = 19` |
| `cAttackPlanMovementIntervalTime` | `const int cAttackPlanMovementIntervalTime = 24` | `const int cAttackPlanMovementIntervalTime = 22` |
| `cAttackPlanNoTargetStartTime` | `const int cAttackPlanNoTargetStartTime = 21` | `const int cAttackPlanNoTargetStartTime = 20` |
| `cAttackPlanNoTargetTimeout` | `const int cAttackPlanNoTargetTimeout = 22` | `const int cAttackPlanNoTargetTimeout = 21` |
| `cDefendPlanGatherPercentage` | `const int cDefendPlanGatherPercentage = 15` | `const int cDefendPlanGatherPercentage = 13` |
| `cDefendPlanMovementIntervalTime` | `const int cDefendPlanMovementIntervalTime = 19` | `const int cDefendPlanMovementIntervalTime = 17` |
| `cDefendPlanNoTargetTimeout` | `const int cDefendPlanNoTargetTimeout = 13` | `const int cDefendPlanNoTargetTimeout = 12` |
| `cDefendPlanPatrol` | `const int cDefendPlanPatrol = 16` | `const int cDefendPlanPatrol = 14` |
| `cDefendPlanPatrolCurrentWaypoint` | `const int cDefendPlanPatrolCurrentWaypoint = 18` | `const int cDefendPlanPatrolCurrentWaypoint = 16` |
| `cDefendPlanPatrolWaypoints` | `const int cDefendPlanPatrolWaypoints = 17` | `const int cDefendPlanPatrolWaypoints = 15` |
| `cTransportPlanDropOffPoint` | `const int cTransportPlanDropOffPoint = 16` | `const int cTransportPlanDropOffPoint = 7` |
| `cTransportPlanGatherPoint` | `const int cTransportPlanGatherPoint = 2` | `const int cTransportPlanGatherPoint = 4` |
| `cTransportPlanReturnWhenDone` | `const int cTransportPlanReturnWhenDone = 10` | `const int cTransportPlanReturnWhenDone = 12` |
| `cTransportPlanTargetPoint` | `const int cTransportPlanTargetPoint = 3` | `const int cTransportPlanTargetPoint = 2` |
| `cTransportPlanTransportPath` | `const int cTransportPlanTransportPath = 20` | `const int cTransportPlanTransportPath = 14` |

</details>

For current usage, look up the declaration and any detailed comments in retail
Doxygen, then check the BANG guide for the intended runtime. See [XS and scenarios](XS_and_Scenarios.md).
