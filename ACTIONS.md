# Shortcuts Actions Reference

Complete catalog of all 427 WF*Action classes and their identifiers.

## Identifier Mapping Rules

### Standard Mapping
Class `WF<Name>Action` maps to `is.workflow.actions.<lowercasename>`

Example: `WFShowResultAction` → `is.workflow.actions.showresult`

### Irregular Mappings

Some actions have non-standard mappings:

| Class Name | Identifier |
|------------|-----------|
| `WFRepeatAction` | `is.workflow.actions.repeat.count` |
| `WFForEachRepeatAction` | `is.workflow.actions.repeat.each` |
| `WFFiniteRepeatAction` | `is.workflow.actions.repeat.count` |
| `WFAskForInputAction` | `is.workflow.actions.ask` |
| `WFTextAction` | `is.workflow.actions.gettext` |
| `WFConditionalAction` | `is.workflow.actions.conditional` |
| `WFChooseFromMenuAction` | `is.workflow.actions.choosefrommenu` |
| `WFGetFileAction` | `is.workflow.actions.documentpicker.open` |
| `WFSelectFilesAction` | `is.workflow.actions.documentpicker.open` |
| `WFSaveFileAction` | `is.workflow.actions.documentpicker.save` |
| `WFGetCurrentWeatherConditionsAction` | `is.workflow.actions.weather.currentconditions` |
| `WFGetWeatherForecastAction` | `is.workflow.actions.weather.forecast` |
| `WFContentItemFilterAction` | `is.workflow.actions.filter.contentitems` |
| `WFGetUpcomingCalendarItemsAction` | `is.workflow.actions.getupcomingevents` |
| `WFAppendFileAction` | `is.workflow.actions.file.append` (was `appendfile` in older versions) |

---

## Actions by Category

### Text & Input

| Identifier | Class | Description |
|------------|-------|-------------|
| `gettext` | WFTextAction | Create a text value |
| `ask` | WFAskForInputAction | Ask user for input |
| `askllm` | WFAskLLMAction | Use AI model (Apple Intelligence) |
| `comment` | WFCommentAction | Add a comment (no effect) |
| `dictatetext` | WFDictateTextAction | Dictate text |
| `showresult` | WFShowResultAction | Display result to user |
| `alert` | WFAlertAction | Show alert dialog |
| `notification` | WFNotificationAction | Send notification |
| `speaktext` | WFSpeakTextAction | Speak text aloud |
| `translatetext` | WFTranslateTextAction | Translate text |
| `detectlanguage` | WFDetectLanguageAction | Detect language |

### Variables

| Identifier | Class | Description |
|------------|-------|-------------|
| `setvariable` | WFSetVariableAction | Set a variable |
| `getvariable` | WFGetVariableAction | Get a variable |
| `appendvariable` | WFAppendVariableAction | Append to variable |
| `nothing` | WFNothingAction | Do nothing (pass-through) |

### Control Flow

| Identifier | Class | Description |
|------------|-------|-------------|
| `repeat.count` | WFRepeatAction | Repeat N times |
| `repeat.each` | WFForEachRepeatAction | Repeat for each item |
| `conditional` | WFConditionalAction | If/Otherwise |
| `choosefrommenu` | WFChooseFromMenuAction | Menu with cases |
| `choosefromlist` | WFChooseFromListAction | Choose from list |
| `exit` | WFExitAction | Exit shortcut |
| `output` | WFOutputAction | Set output |

### Files & Documents

| Identifier | Class | Description |
|------------|-------|-------------|
| `file` | WFFileAction | Create file reference |
| `documentpicker.open` | WFSelectFilesAction | Open file picker |
| `documentpicker.save` | WFSaveFileAction | Save file |
| `getfoldercontents` | WFGetFolderContentsAction | List folder contents |
| `createfolder` | WFCreateFolderAction | Create folder |
| `deletefile` | WFDeleteFileAction | Delete file |
| `movefile` | WFMoveFileAction | Move file |
| `renamefile` | WFRenameFileAction | Rename file |
| `file.append` | WFAppendFileAction | Append to text file (was `appendfile` in older versions) |
| `makearchive` | WFMakeArchiveAction | Create archive |
| `extractarchive` | WFExtractArchiveAction | Extract archive |

### Web & URLs

| Identifier | Class | Description |
|------------|-------|-------------|
| `url` | WFURLAction | Create URL |
| `downloadurl` | WFDownloadURLAction | Get contents of URL |
| `openurl` | WFOpenURLAction | Open URL |
| `expandurl` | WFExpandURLAction | Expand shortened URL |
| `geturlheaders` | WFGetURLHeadersAction | Get URL headers |
| `urlgetcomponent` | WFURLGetComponentAction | Get URL component |
| `urlencode` | WFURLEncodeAction | URL encode |
| `getwebpage` | WFGetWebPageAction | Get web page |
| `searchweb` | WFSearchWebAction | Search web |

### Apps & System

| Identifier | Class | Description |
|------------|-------|-------------|
| `openapp` | WFOpenAppAction | Open app |
| `quitapp` | WFQuitAppAction | Quit app |
| `hideapp` | WFHideAppAction | Hide app |
| `getcurrentapp` | WFGetCurrentAppAction | Get current app |
| `runworkflow` | WFRunWorkflowAction | Run another shortcut |
| `runshellscript` | WFRunShellScriptAction | Run shell script |
| `runosascript` | WFRunOSAScriptAction | Run AppleScript |
| `getdevicedetails` | WFGetDeviceDetailsAction | Get device info |
| `batterylevel` | WFBatteryLevelAction | Get battery level |
| `getclipboard` | WFGetClipboardAction | Get clipboard |
| `setclipboard` | WFSetClipboardAction | Set clipboard |

### Lists & Data

| Identifier | Class | Description |
|------------|-------|-------------|
| `list` | WFListAction | Create list |
| `dictionary` | WFDictionaryAction | Create dictionary |
| `getdictionaryvalue` | WFGetDictionaryValueAction | Get dictionary value |
| `setdictionaryvalue` | WFSetDictionaryValueAction | Set dictionary value |
| `getitemfromlist` | WFGetItemFromListAction | Get item from list |
| `count` | WFCountAction | Count items |
| `filter.contentitems` | WFContentItemFilterAction | Filter content |

### Numbers & Math

| Identifier | Class | Description |
|------------|-------|-------------|
| `number` | WFNumberAction | Create number |
| `calculate` | WFCalculateAction | Calculate |
| `calculatestatistics` | WFCalculateStatisticsAction | Statistics |
| `randomnumber` | WFRandomNumberAction | Random number |
| `roundnumber` | WFRoundNumberAction | Round number |
| `measurementcreate` | WFMeasurementCreateAction | Create measurement |
| `measurementconvert` | WFMeasurementConvertAction | Convert measurement |

### Date & Time

| Identifier | Class | Description |
|------------|-------|-------------|
| `date` | WFDateAction | Create date |
| `formatdate` | WFFormatDateAction | Format date |
| `adjustdate` | WFAdjustDateAction | Adjust date |
| `converttimezone` | WFConvertTimeZoneAction | Convert timezone |
| `timeuntildate` | WFTimeUntilDateAction | Time between dates |
| `delay` | WFDelayAction | Wait |
| `waittoreturn` | WFWaitToReturnAction | Wait to return |

### Calendar & Reminders

| Identifier | Class | Description |
|------------|-------|-------------|
| `addnewevent` | WFAddNewEventAction | Create event |
| `getupcomingevents` | WFGetUpcomingCalendarItemsAction | Get upcoming events |
| `removecalendaritems` | WFRemoveCalendarItemsAction | Remove calendar items |
| `addnewreminder` | WFAddNewReminderAction | Create reminder |
| `showreminderslist` | WFShowRemindersListAction | Show reminders |

### Weather & Location

| Identifier | Class | Description |
|------------|-------|-------------|
| `weather.currentconditions` | WFGetCurrentWeatherConditionsAction | Current weather |
| `weather.forecast` | WFGetWeatherForecastAction | Weather forecast |
| `getcurrentlocation` | WFGetCurrentLocationAction | Current location |
| `location` | WFLocationAction | Create location |
| `getdirections` | WFGetDirectionsAction | Get directions |
| `getdistance` | WFGetDistanceAction | Get distance |
| `searchmaps` | WFSearchMapsAction | Search maps |

### Media

| Identifier | Class | Description |
|------------|-------|-------------|
| `takephoto` | WFTakePhotoAction | Take photo |
| `takevideo` | WFTakeVideoAction | Take video |
| `selectphoto` | WFSelectPhotoAction | Select photos |
| `getlatestphotos` | WFGetLatestPhotosAction | Get latest photos |
| `savetocameraroll` | WFSaveToCameraRollAction | Save to camera roll |
| `deletephotos` | WFDeletePhotosAction | Delete photos |
| `playmusic` | WFPlayMusicAction | Play music |
| `playpause` | WFPlayPauseAction | Play/Pause |
| `skipsong` | WFSkipSongAction | Skip song |
| `recordaudio` | WFRecordAudioAction | Record audio |
| `playsound` | WFPlaySoundAction | Play sound |

### Images

| Identifier | Class | Description |
|------------|-------|-------------|
| `imageresize` | WFImageResizeAction | Resize image |
| `imagecrop` | WFImageCropAction | Crop image |
| `imagerotate` | WFImageRotateAction | Rotate image |
| `imageflip` | WFImageFlipAction | Flip image |
| `imageconvert` | WFImageConvertAction | Convert image |
| `imagecombine` | WFImageCombineAction | Combine images |
| `overlayimage` | WFOverlayImageAction | Overlay image |
| `overlaytext` | WFOverlayTextAction | Overlay text |
| `imageremovebackground` | WFImageRemoveBackgroundAction | Remove background |
| `maskimage` | WFMaskImageAction | Mask image |
| `extracttextfromimage` | WFExtractTextFromImageAction | OCR |

### PDF

| Identifier | Class | Description |
|------------|-------|-------------|
| `makepdf` | WFMakePDFAction | Create PDF |
| `splitpdf` | WFSplitPDFAction | Split PDF |
| `compresspdf` | WFCompressPDFAction | Compress PDF |
| `gettextfrompdf` | WFGetTextFromPDFAction | Extract text from PDF |
| `makeimagefrompdfpage` | WFMakeImageFromPDFPageAction | PDF page to image |

### Sharing & Communication

| Identifier | Class | Description |
|------------|-------|-------------|
| `share` | WFShareAction | Share |
| `airdrop` | WFAirDropAction | AirDrop |
| `sendmessage` | WFSendMessageAction | Send message |
| `sendemail` | WFSendEmailAction | Send email |
| `startcall` | WFStartCallAction | Start call |
| `contacts` | WFContactsAction | Get contacts |
| `selectcontacts` | WFSelectContactsAction | Select contacts |

### Settings

| Identifier | Class | Description |
|------------|-------|-------------|
| `setappearance` | WFSetAppearanceAction | Set light/dark mode |
| `setwifi` | WFSetWiFiAction | Set WiFi |
| `setcellulardata` | WFSetCellularDataAction | Set cellular data |
| `setlowpowermode` | WFSetLowPowerModeAction | Set low power mode |
| `setvolume` | WFSetVolumeAction | Set volume |
| `toggledonotdisturb` | WFToggleDoNotDisturbAction | Toggle Do Not Disturb |
| `setorientationlock` | WFSetOrientationLockAction | Set orientation lock |
| `setwallpaper` | WFSetWallpaperAction | Set wallpaper |

---

## Complete Identifier List

All 427 action identifiers (prefix `is.workflow.actions.` omitted):

```
addframetogif, addmusictoupnext, addnewcalendar, addnewcontact, addnewevent,
addnewreminder, addquickreminder, address, addtoplaylist, addtoreadinglist,
adjustdate, airdrop, alert, appattributed, appenddropboxfile, file.append,
appendtonote, appendvariable, appintentexecution, ask, askllm, batterylevel,
calculate, calculateexpression, calculatestatistics, changeplaybackdestination,
choosefromlist, choosefrommenu, clearupnext, coercion, comment, compactdialog,
compresspdf, conditional, configuredactionbuttonintent, configuredactionbuttonnothing,
configuredactionbuttonworkflow, configuredstaccato, configuredstaccatointent,
configuredstaccatonothing, configuredstaccatotophit, configuredstaccatoworkflow,
configuredsystem, configuredsystemcontrol, configuredsystemintent,
configuredsystemnothing, configuredsystemworkflow, connecttoservers, contacts,
contentattributionsetdebugger, contentitem, contentitemproperties, contentitemsetter,
controlflow, converttimezone, count, createfolder, createnote, createphotoalbum,
createplaylist, date, delay, deletefile, deletephotos, detectlanguage, dictatetext,
dictionary, displaysleep, documentpicker.open, documentpicker.save, downloadurl,
ejectdisk, emailaddress, encodemedia, evernoteappend, evernotecreate, evernotedelete,
evernotegetlink, evernotegetnotes, exit, expandurl, extractarchive,
extracttextfromimage, file, filter.contentitems, finderimageconvert,
findhealthsamples, focusconfigurationlink, folder, formatdate, formatfilesize,
formatnumber, generatehash, generatemachinereadablecode, getclass, getclipboard,
getcurrentapp, getcurrentlocation, getcurrentsafariwebpage, getcurrentsong,
getdevicedetails, getdictionaryvalue, getdirections, getdistance, getdropboxfile,
getemojiname, getepisodesforpodcast, getfilelink, getfocus, getfoldercontents,
getframesfromimage, gethalfwaypoint, gethomeaccessorystate, gethotspotpassword,
getipaddress, getitemfromlist, getitemname, getitemtype, getlatestphotoimport,
getlatestphotos, getmapslink, getmyworkflows, getnetworkdetails, getonscreencontent,
getparentdirectory, getparkedcarlocation, getplaylist, getpodcastsfromlibrary,
getposters, getselectedfinderfiles, gettext, gettextfrompdf, gettraveltime,
gettype, getupcomingevents, geturlheaders, getvariable, getwebpage, giphy,
handlecustomintent, handledonatedintent, handleintent, handlepaymentintent,
handlesystemintent, handoff, handoffplayback, hideapp, homeaccessory,
htmlfromrichtext, imagecombine, imageconvert, imagecrop, imageflip,
imageremovebackground, imageresize, imagerotate, imgurupload, importaudiofiles,
importtolightroom, input, instapaper, instapaperadd, instapaperget, interchange,
interchangescheme, intercom, labelfiles, link, linkactionserializedparametersforln,
linkbookschangepagenavigation, linkbookschangetheme, linkbooksfind,
linkbooksnavigatepages, linkcalculateappusageintent, linkcalendarclosescreen,
linkcalendarcreatecalendar, linkcalendardeletecalendar, linkcalendaropenscreen,
linkchangebinarysetting, linkclockcreatealarm, linkclockdeletealarm,
linkclocktogglealarm, linkcloseentity, linkcontentitemfilter, linkcopyentity,
linkcreateentity, linkdeleteentity, linkentity, linkfavoriteentity, linkfindhome,
linkfindhomecameraclip, linkfindhomedevice, linkfindhomeroom, linkfindhomescene,
linkfindhomezone, linkfindselectedhome, linkimageplaygroundgenerateimage,
linkinsertintelligencetext, linkipdatafindsportsevents,
linkmusicrecognitionrecognizemusic, linknavigatesequentially,
linknotesaddtagstonotes, linknoteschangesetting, linknotescreatefolder,
linknotescreatetag, linknotesdeletefolders, linknotesdeletetags, linknotesfind,
linknotesmovenotestofolder, linknotesopenaccount, linknotesopenapplocation,
linknotesopenfolder, linknotesopentag, linknotespinnotes,
linknotesremovetagsfromnotes, linkopencamera, linkopenentity,
linkphotoscreatememory, linkreminderscreatelist, linkremindersopensmartlist,
linkrunintelligencecommand, linksafarichangereadermodestate, linksafariclosetab,
linksafaricreateprivatetab, linksafaricreatetab, linksafaricreatetabgroup,
linksafarifindbookmarks, linksafarifindreadinglistitems, linksafarifindtabgroups,
linksafarifindtabs, linksafariopenbookmark, linksafariopenreadinglistitem,
linksafariopentab, linksafariopentabgroup, linksafariopenview, linksearch,
linkshortcutscreateicloudlink, linkshortcutscreateworkflow,
linkshortcutsdeleteworkflow, linkshortcutsresetcellulardatastatistics,
linkshortcutssearchshortcuts, linkshortcutssetdataroaming, linkshortcutssetdefaultline,
linkshortcutstogglecellularplan, linkstartstopwatch, linkstartworkout,
linktogglehomeaccessory, linkvisualintelligencecamera,
linkvoicememoschangerecordingplaybacksetting, linkvoicememoscreatefolder,
linkvoicememosdeletefolders, linkvoicememosdeleterecordings, linkvoicememosopenfolder,
linkvoicememosopenrecording, linkvoicememosplayrecording, linkvoicememosrecordingfind,
linkvoicememossearchrecordings, linkwritingtools, linkwritingtoolsadjusttone,
linkwritingtoolsformatlist, linkwritingtoolsformattable, linkwritingtoolsproofread,
linkwritingtoolsrewrite, linkwritingtoolssummarize, list, location, lockapp,
lockscreen, loghealthsample, logoutuser, logworkout, makearchive, makediskimage,
makegif, makeimagefrompdfpage, makeimagefromrichtext, makepdf,
makespokenaudiofromtext, makevideofromgif, markdownfromrichtext, markup, maskimage,
measurementconvert, measurementcreate, missing, mountdiskimage, movefile, movewindow,
nothing, notification, number, openapp, openin, openincalendar, openurl,
openuseractivity, openxcallbackurl, output, overlayimage, overlaytext,
overridablelink, phonenumber, pinboardadd, pinboardget, playmusic, playpause,
playpodcast, playsound, pocketadd, pocketget, print, quicklook, quitapp,
randomnumber, recognizemusic, recordaudio, remoteappintentexecution, remotelink,
removecalendaritems, removephotofromalbum, renamefile, repeat.count, repeat.each,
replacetext, requestrideintent, requestuber, resizewindow, returntohomescreen,
revealfiles, reversiblelink, richtextfromhtml, richtextfrommarkdown, roundnumber,
rssfeed, rssfeedextract, runjavascriptonwebpage, runosascript, runshellscript,
runshortcutconfigurationintent, runshortcutintent, runsshscript, runworkflow,
savedropboxfile, savetocameraroll, scanmachinereadablecode, searchitunes,
searchlocalbusinesses, searchmaps, searchweb, seek, selectcontacts, selectmusic,
selectphoto, sendemail, sendmessage, sendtogoodreader, setairdropreceiving,
setalwaysondisplay, setappearance, setcellulardata, setclipboard, setdictionaryvalue,
sethotspotpassword, setitemname, setlisteningmode, setlowpowermode, setorientationlock,
setparkedcar, setvariable, setvolume, setvpn, setwallpaper, setwifi, share,
shareextension, shazammedia, showdefinition, showinblindsquare, showinstore, shownote,
showpasswords, showreminderslist, showresult, showwebpage, shutdowndevice, skipsong,
sleepdevice, social, speaktext, splitpdf, splitscreenapp, spotlightsearch,
staccatolink, standaloneshortcut, startcall, startscreensaver, starttimer,
storageservice, storageserviceinput, subscribetopodcast, switchposter, takephoto,
takescreenshot, takevideo, textcomponents, timeuntildate, todoistadd,
toggledonotdisturb, translatetext, trelloaddcard, trellocreateboard, trellocreatelist,
trellogetitems, trimvideo, trimwhitespace, tumblrpost, ulyssesattach, url, urlencode,
urlgetcomponent, vibrate, viewcontentgraph, waittoreturn, watchmedo,
weather.currentconditions, weather.forecast, wordpresspost
```

---

## Common Parameter Patterns

### Text Parameters
```xml
<key>WFTextActionText</key>
<string>Your text here</string>
```

### Variable Reference Parameters
```xml
<key>Text</key>
<dict>
    <key>Value</key>
    <dict>
        <key>attachmentsByRange</key>
        <dict>
            <key>{0, 1}</key>
            <dict>
                <key>OutputUUID</key>
                <string>SOURCE-UUID</string>
                <key>OutputName</key>
                <string>Text</string>
                <key>Type</key>
                <string>ActionOutput</string>
            </dict>
        </dict>
        <key>string</key>
        <string>￼</string>
    </dict>
    <key>WFSerializationType</key>
    <string>WFTextTokenString</string>
</dict>
```

### Boolean Parameters
```xml
<key>WFSomeOption</key>
<true/>
```

### Number Parameters
```xml
<key>WFRepeatCount</key>
<integer>5</integer>
```

### Enum Parameters
```xml
<key>WFHTTPMethod</key>
<string>GET</string>
```
