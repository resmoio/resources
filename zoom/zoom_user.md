---
description: Zoom User
---
zoom_user
---------

| **Name**          | **Type**           | **Nullable** |
| ----------------- | ------------------ | ------------ |
| createdAt         | String             | &check;      |
| customAttributes  | Map<String,String> | &check;      |
| dept              | String             | &check;      |
| email             | String             | &check;      |
| employeeUniqueId  | String             | &check;      |
| firstName         | String             | &check;      |
| groupIds          | List<String>       | &check;      |
| id                | String             | &cross;      |
| imGroupIds        | List<String>       | &check;      |
| lastClientVersion | String             | &check;      |
| lastLoginTime     | String             | &check;      |
| lastName          | String             | &check;      |
| permissions       | List<String>       | &check;      |
| planUnitedType    | String             | &check;      |
| pmi               | String             | &check;      |
| roleId            | String             | &check;      |
| status            | String             | &check;      |
| timezone          | String             | &check;      |
| type              | Int                | &check;      |
| userSettings      | UserSettings       | &check;      |
| verified          | Int                | &check;      |

#### UserSettings
| **Name**                        | **Type**                                     | **Nullable** |
| ------------------------------- | -------------------------------------------- | ------------ |
| audioConferencing               | UserSettings.AudioConferencing               | &check;      |
| emailNotification               | Map<String,Boolean>                          | &check;      |
| feature                         | UserSettings.Feature                         | &check;      |
| inMeeting                       | UserSettings.InMeeting                       | &check;      |
| meetingAuthenticationSettings   | UserSettings.MeetingAuthenticationSettings   | &check;      |
| meetingSecuritySettings         | UserSettings.MeetingSecuritySettings         | &check;      |
| profile                         | UserSettings.Profile                         | &check;      |
| recordingAuthenticationSettings | UserSettings.RecordingAuthenticationSettings | &check;      |
| scheduleMeeting                 | UserSettings.ScheduleMeeting                 | &check;      |
| telephony                       | UserSettings.Telephony                       | &check;      |
| tsp                             | UserSettings.Tsp                             | &check;      |

#### UserSettings.AudioConferencing
| **Name**                  | **Type**                                                 | **Nullable** |
| ------------------------- | -------------------------------------------------------- | ------------ |
| tollFreeAndFeeBasedToCall | UserSettings.AudioConferencing.TollFreeAndFeeBasedToCall | &check;      |

#### UserSettings.AudioConferencing.TollFreeAndFeeBasedToCall
| **Name**                  | **Type**  | **Nullable** |
| ------------------------- | --------- | ------------ |
| allowWebinarAttendeesDial | Boolean   | &check;      |
| enable                    | Boolean   | &check;      |
| numbers                   | List<Map> | &check;      |

#### UserSettings.Feature
| **Name**               | **Type** | **Nullable** |
| ---------------------- | -------- | ------------ |
| concurrentMeeting      | String   | &check;      |
| largeMeeting           | Boolean  | &check;      |
| largeMeetingCapacity   | Int      | &check;      |
| meetingCapacity        | Int      | &check;      |
| webinar                | Boolean  | &check;      |
| webinarCapacity        | Int      | &check;      |
| zoomCustomerManagedKey | Boolean  | &check;      |
| zoomEvents             | Boolean  | &check;      |
| zoomEventsCapacity     | Int      | &check;      |
| zoomIqForSales         | Boolean  | &check;      |
| zoomPhone              | Boolean  | &check;      |
| zoomTranslatedCaptions | Boolean  | &check;      |
| zoomWhiteboard         | Boolean  | &check;      |
| zoomWhiteboardPlus     | Boolean  | &check;      |

#### UserSettings.InMeeting
| **Name**                                | **Type**                                         | **Nullable** |
| --------------------------------------- | ------------------------------------------------ | ------------ |
| allowHostPanelistsToUseAudibleClap      | Boolean                                          | &check;      |
| allowHostToEnableFocusMode              | Boolean                                          | &check;      |
| allowLiveStreaming                      | Boolean                                          | &check;      |
| allowParticipantsChatWith               | Int                                              | &check;      |
| allowUsersSaveChats                     | Int                                              | &check;      |
| allowUsersToDeleteMessagesInMeetingChat | Boolean                                          | &check;      |
| annotation                              | Boolean                                          | &check;      |
| attentionModeFocusMode                  | Boolean                                          | &check;      |
| autoSavingChat                          | Boolean                                          | &check;      |
| breakoutRoom                            | Boolean                                          | &check;      |
| breakoutRoomSchedule                    | Boolean                                          | &check;      |
| chat                                    | Boolean                                          | &check;      |
| closedCaption                           | Boolean                                          | &check;      |
| closedCaptioning                        | Map<String,Boolean>                              | &check;      |
| coHost                                  | Boolean                                          | &check;      |
| customDataCenterRegions                 | Boolean                                          | &check;      |
| customLiveStreamingService              | Boolean                                          | &check;      |
| customServiceInstructions               | String                                           | &check;      |
| dataCenterRegions                       | List<String>                                     | &check;      |
| disableScreenSharingForHostMeetings     | Boolean                                          | &check;      |
| disableScreenSharingForInMeetingGuests  | Boolean                                          | &check;      |
| e2eEncryption                           | Boolean                                          | &check;      |
| entryExitChime                          | String                                           | &check;      |
| farEndCameraControl                     | Boolean                                          | &check;      |
| feedback                                | Boolean                                          | &check;      |
| fileTransfer                            | Boolean                                          | &check;      |
| groupHd                                 | Boolean                                          | &check;      |
| joinFromDesktop                         | Boolean                                          | &check;      |
| joinFromMobile                          | Boolean                                          | &check;      |
| languageInterpretation                  | UserSettings.InMeeting.LanguageInterpretation    | &check;      |
| liveStreamingFacebook                   | Boolean                                          | &check;      |
| liveStreamingYoutube                    | Boolean                                          | &check;      |
| manualCaptioning                        | Map<String,Boolean>                              | &check;      |
| meetingPolling                          | Map<String,Boolean>                              | &check;      |
| meetingReactions                        | Boolean                                          | &check;      |
| meetingReactionsEmojis                  | String                                           | &check;      |
| meetingSurvey                           | Boolean                                          | &check;      |
| nonVerbalFeedback                       | Boolean                                          | &check;      |
| participantsShareSimultaneously         | String                                           | &check;      |
| polling                                 | Boolean                                          | &check;      |
| postMeetingFeedback                     | Boolean                                          | &check;      |
| privateChat                             | Boolean                                          | &check;      |
| recordPlayVoice                         | Boolean                                          | &check;      |
| recording                               | UserSettings.Recording                           | &check;      |
| remoteControl                           | Boolean                                          | &check;      |
| remoteSupport                           | Boolean                                          | &check;      |
| requestPermissionToUnmute               | Boolean                                          | &check;      |
| screenSharing                           | Boolean                                          | &check;      |
| showAJoinFromYourBrowserLink            | Boolean                                          | &check;      |
| showMeetingControlToolbar               | Boolean                                          | &check;      |
| slideControl                            | Boolean                                          | &check;      |
| uncheckedDataCenterRegions              | List<String>                                     | &check;      |
| virtualBackground                       | Boolean                                          | &check;      |
| virtualBackgroundSettings               | UserSettings.InMeeting.VirtualBackgroundSettings | &check;      |
| waitingRoom                             | Boolean                                          | &check;      |
| webinarChat                             | UserSettings.InMeeting.WebinarChat               | &check;      |
| webinarLiveStreaming                    | UserSettings.InMeeting.WebinarLiveStreaming      | &check;      |
| webinarPolling                          | Map<String,Boolean>                              | &check;      |
| webinarReactions                        | Boolean                                          | &check;      |
| webinarSurvey                           | Boolean                                          | &check;      |
| whiteboard                              | Boolean                                          | &check;      |
| whoCanShareScreen                       | String                                           | &check;      |
| whoCanShareScreenWhenSomeoneIsSharing   | String                                           | &check;      |
| workplaceByFacebook                     | Boolean                                          | &check;      |

#### UserSettings.InMeeting.LanguageInterpretation
| **Name**                                         | **Type**     | **Nullable** |
| ------------------------------------------------ | ------------ | ------------ |
| allowParticipantsToSpeakInListeningChannel       | Boolean      | &check;      |
| allowUpTo25CustomLanguagesWhenSchedulingMeetings | Boolean      | &check;      |
| customLanguages                                  | List<String> | &check;      |
| enable                                           | Boolean      | &check;      |
| enableLanguageInterpretationByDefault            | Boolean      | &check;      |
| languages                                        | List<String> | &check;      |

#### UserSettings.InMeeting.VirtualBackgroundSettings
| **Name**          | **Type**                                                    | **Nullable** |
| ----------------- | ----------------------------------------------------------- | ------------ |
| allowUploadCustom | Boolean                                                     | &check;      |
| allowVideos       | Boolean                                                     | &check;      |
| enable            | Boolean                                                     | &check;      |
| files             | List<UserSettings.InMeeting.VirtualBackgroundSettings.File> | &check;      |

#### UserSettings.InMeeting.VirtualBackgroundSettings.File
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| isDefault | Boolean  | &check;      |
| name      | String   | &check;      |
| size      | Int      | &check;      |
| type      | String   | &check;      |

#### UserSettings.InMeeting.WebinarChat
| **Name**                        | **Type** | **Nullable** |
| ------------------------------- | -------- | ------------ |
| allowAttendeesChatWith          | Int      | &check;      |
| allowAutoSaveLocalChatFile      | Boolean  | &check;      |
| allowPanelistsChatWith          | Int      | &check;      |
| allowPanelistsSendDirectMessage | Boolean  | &check;      |
| allowUsersSaveChats             | Int      | &check;      |
| defaultAttendeesChatWith        | Int      | &check;      |
| enable                          | Boolean  | &check;      |

#### UserSettings.InMeeting.WebinarLiveStreaming
| **Name**                  | **Type**     | **Nullable** |
| ------------------------- | ------------ | ------------ |
| customServiceInstructions | String       | &check;      |
| enable                    | Boolean      | &check;      |
| liveStreamingReminder     | Boolean      | &check;      |
| liveStreamingService      | List<String> | &check;      |

#### UserSettings.MeetingAuthenticationSettings
| **Name**                     | **Type**                                                               | **Nullable** |
| ---------------------------- | ---------------------------------------------------------------------- | ------------ |
| allowAuthenticationException | Boolean                                                                | &check;      |
| authenticationOptions        | List<UserSettings.MeetingAuthenticationSettings.AuthenticationOptions> | &check;      |
| meetingAuthentication        | Boolean                                                                | &check;      |

#### UserSettings.MeetingAuthenticationSettings.AuthenticationOptions
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| defaultOption | Boolean  | &check;      |
| domains       | String   | &check;      |
| id            | String   | &check;      |
| name          | String   | &check;      |
| type          | String   | &check;      |
| visible       | Boolean  | &check;      |

#### UserSettings.MeetingSecuritySettings
| **Name**                              | **Type**                                                        | **Nullable** |
| ------------------------------------- | --------------------------------------------------------------- | ------------ |
| autoSecurity                          | Boolean                                                         | &check;      |
| blockUserDomain                       | Boolean                                                         | &check;      |
| blockUserDomainList                   | List<String>                                                    | &check;      |
| embedPasswordInJoinLink               | Boolean                                                         | &check;      |
| encryptionType                        | String                                                          | &check;      |
| endToEndEncryptedMeetings             | Boolean                                                         | &check;      |
| meetingPassword                       | Boolean                                                         | &check;      |
| meetingPasswordRequirement            | UserSettings.MeetingSecuritySettings.MeetingPasswordRequirement | &check;      |
| onlyAuthenticatedCanJoinFromWebclient | Boolean                                                         | &check;      |
| phonePassword                         | Boolean                                                         | &check;      |
| pmiPassword                           | Boolean                                                         | &check;      |
| requirePasswordForScheduledMeeting    | Boolean                                                         | &check;      |
| requirePasswordForScheduledWebinar    | Boolean                                                         | &check;      |
| waitingRoom                           | Boolean                                                         | &check;      |
| waitingRoomSettings                   | UserSettings.MeetingSecuritySettings.WaitingRoomSettings        | &check;      |
| webinarPassword                       | Boolean                                                         | &check;      |

#### UserSettings.MeetingSecuritySettings.MeetingPasswordRequirement
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| consecutiveCharactersLength | Int      | &check;      |
| haveLetter                  | Boolean  | &check;      |
| haveNumber                  | Boolean  | &check;      |
| haveSpecialCharacter        | Boolean  | &check;      |
| haveUpperAndLowerCharacters | Boolean  | &check;      |
| length                      | Int      | &check;      |
| onlyAllowNumeric            | Boolean  | &check;      |
| weakEnhanceDetection        | Boolean  | &check;      |

#### UserSettings.MeetingSecuritySettings.WaitingRoomSettings
| **Name**                                    | **Type** | **Nullable** |
| ------------------------------------------- | -------- | ------------ |
| participantsToPlaceInWaitingRoom            | Int      | &check;      |
| usersWhoCanAdmitParticipantsFromWaitingRoom | Int      | &check;      |
| whitelistedDomainsForWaitingRoom            | Int      | &check;      |

#### UserSettings.Profile
| **Name**                 | **Type**                                      | **Nullable** |
| ------------------------ | --------------------------------------------- | ------------ |
| recordingStorageLocation | UserSettings.Profile.RecordingStorageLocation | &check;      |

#### UserSettings.Profile.RecordingStorageLocation
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| allowedValues | List<String> | &check;      |
| value         | String       | &check;      |

#### UserSettings.Recording
| **Name**                                | **Type**                                            | **Nullable** |
| --------------------------------------- | --------------------------------------------------- | ------------ |
| askHostToConfirmDisclaimer              | Boolean                                             | &check;      |
| askParticipantsToConsentDisclaimer      | Boolean                                             | &check;      |
| autoDeleteCmr                           | Boolean                                             | &check;      |
| autoDeleteCmrDays                       | Int                                                 | &check;      |
| autoRecording                           | String                                              | &check;      |
| cloudRecording                          | Boolean                                             | &check;      |
| displayParticipantName                  | Boolean                                             | &check;      |
| hostPauseStopRecording                  | Boolean                                             | &check;      |
| ipAddressAccessControl                  | UserSettings.Recording.IpAddressAccessControl       | &check;      |
| localRecording                          | Boolean                                             | &check;      |
| optimizeRecordingFor3rdPartyVideoEditor | Boolean                                             | &check;      |
| recordAudioFile                         | Boolean                                             | &check;      |
| recordFilesSeparately                   | Map<String,Boolean>                                 | &check;      |
| recordGalleryView                       | Boolean                                             | &check;      |
| recordSpeakerView                       | Boolean                                             | &check;      |
| recordingAudioTranscript                | Boolean                                             | &check;      |
| recordingDisclaimer                     | Boolean                                             | &check;      |
| recordingPasswordRequirement            | UserSettings.Recording.RecordingPasswordRequirement | &check;      |
| recordingThumbnails                     | Boolean                                             | &check;      |
| saveChatText                            | Boolean                                             | &check;      |
| saveCloseCaption                        | Boolean                                             | &check;      |
| savePanelistChat                        | Boolean                                             | &check;      |
| savePollResults                         | Boolean                                             | &check;      |
| showTimestamp                           | Boolean                                             | &check;      |
| smartRecording                          | Map<String,Boolean>                                 | &check;      |

#### UserSettings.Recording.IpAddressAccessControl
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| enable              | Boolean  | &check;      |
| ipAddressesOrRanges | String   | &check;      |

#### UserSettings.Recording.RecordingPasswordRequirement
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| haveLetter           | Boolean  | &check;      |
| haveNumber           | Boolean  | &check;      |
| haveSpecialCharacter | Boolean  | &check;      |
| length               | Int      | &check;      |
| onlyAllowNumeric     | Boolean  | &check;      |

#### UserSettings.RecordingAuthenticationSettings
| **Name**                | **Type**                                                                 | **Nullable** |
| ----------------------- | ------------------------------------------------------------------------ | ------------ |
| authenticationOptions   | List<UserSettings.RecordingAuthenticationSettings.AuthenticationOptions> | &check;      |
| recordingAuthentication | Boolean                                                                  | &check;      |

#### UserSettings.RecordingAuthenticationSettings.AuthenticationOptions
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| defaultOption | Boolean  | &check;      |
| domains       | String   | &check;      |
| id            | String   | &check;      |
| name          | String   | &check;      |
| type          | String   | &check;      |
| visible       | Boolean  | &check;      |

#### UserSettings.ScheduleMeeting
| **Name**                                | **Type**                                                | **Nullable** |
| --------------------------------------- | ------------------------------------------------------- | ------------ |
| audioType                               | String                                                  | &check;      |
| defaultPasswordForScheduledMeetings     | String                                                  | &check;      |
| embedPasswordInJoinLink                 | Boolean                                                 | &check;      |
| forcePmiJbhPassword                     | Boolean                                                 | &check;      |
| hostVideo                               | Boolean                                                 | &check;      |
| joinBeforeHost                          | Boolean                                                 | &check;      |
| meetingPasswordRequirement              | UserSettings.ScheduleMeeting.MeetingPasswordRequirement | &check;      |
| participantsVideo                       | Boolean                                                 | &check;      |
| personalMeeting                         | Boolean                                                 | &check;      |
| pmiPassword                             | String                                                  | &check;      |
| pstnPasswordProtected                   | Boolean                                                 | &check;      |
| requirePasswordForInstantMeetings       | Boolean                                                 | &check;      |
| requirePasswordForPmiMeetings           | String                                                  | &check;      |
| requirePasswordForScheduledMeetings     | Boolean                                                 | &check;      |
| requirePasswordForSchedulingNewMeetings | Boolean                                                 | &check;      |
| usePmiForInstantMeetings                | Boolean                                                 | &check;      |
| usePmiForScheduledMeetings              | Boolean                                                 | &check;      |

#### UserSettings.ScheduleMeeting.MeetingPasswordRequirement
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| consecutiveCharactersLength | Int      | &check;      |
| haveLetter                  | Boolean  | &check;      |
| haveNumber                  | Boolean  | &check;      |
| haveSpecialCharacter        | Boolean  | &check;      |
| haveUpperAndLowerCharacters | Boolean  | &check;      |
| length                      | Int      | &check;      |
| onlyAllowNumeric            | Boolean  | &check;      |
| weakEnhanceDetection        | Boolean  | &check;      |

#### UserSettings.Telephony
| **Name**                     | **Type**                                | **Nullable** |
| ---------------------------- | --------------------------------------- | ------------ |
| audioConferenceInfo          | String                                  | &check;      |
| showInternationalNumbersLink | Boolean                                 | &check;      |
| telephonyRegions             | UserSettings.Telephony.TelephonyRegions | &check;      |

#### UserSettings.Telephony.TelephonyRegions
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| allowedValues   | List<String> | &check;      |
| selectionValues | String       | &check;      |
| thirdPartyAudio | String       | &check;      |

#### UserSettings.Tsp
| **Name**                     | **Type**     | **Nullable** |
| ---------------------------- | ------------ | ------------ |
| callOut                      | Boolean      | &check;      |
| callOutCountries             | List<String> | &check;      |
| showInternationalNumbersLink | Boolean      | &check;      |
