---
description: Zoom Account Settings
---
zoom_account_settings
---------------------

| **Name**                        | **Type**                        | **Nullable** |
| ------------------------------- | ------------------------------- | ------------ |
| audioConferencing               | AudioConferencing               | &check;      |
| emailNotification               | Map<String,Boolean>             | &check;      |
| feature                         | Feature                         | &check;      |
| inMeeting                       | InMeeting                       | &check;      |
| integration                     | Map<String,Boolean>             | &check;      |
| meetingAuthenticationSettings   | MeetingAuthenticationSettings   | &check;      |
| meetingSecuritySettings         | MeetingSecuritySettings         | &check;      |
| otherOptions                    | OtherOptions                    | &check;      |
| profile                         | Profile                         | &check;      |
| recording                       | Recording                       | &check;      |
| recordingAuthenticationSettings | RecordingAuthenticationSettings | &check;      |
| scheduleMeeting                 | ScheduleMeeting                 | &check;      |
| security                        | Security                        | &check;      |
| telephony                       | Telephony                       | &check;      |
| tsp                             | Tsp                             | &check;      |
| zoomRooms                       | Map<String,Boolean>             | &check;      |

#### AudioConferencing
| **Name**                  | **Type**                                    | **Nullable** |
| ------------------------- | ------------------------------------------- | ------------ |
| tollFreeAndFeeBasedToCall | AudioConferencing.TollFreeAndFeeBasedToCall | &check;      |

#### AudioConferencing.TollFreeAndFeeBasedToCall
| **Name**                  | **Type**  | **Nullable** |
| ------------------------- | --------- | ------------ |
| allowWebinarAttendeesDial | Boolean   | &check;      |
| enable                    | Boolean   | &check;      |
| numbers                   | List<Map> | &check;      |

#### Feature
| **Name**        | **Type** | **Nullable** |
| --------------- | -------- | ------------ |
| meetingCapacity | Int      | &check;      |

#### InMeeting
| **Name**                                | **Type**                            | **Nullable** |
| --------------------------------------- | ----------------------------------- | ------------ |
| alertGuestJoin                          | Boolean                             | &check;      |
| allowHostPanelistsToUseAudibleClap      | Boolean                             | &check;      |
| allowHostToEnableFocusMode              | Boolean                             | &check;      |
| allowLiveStreaming                      | Boolean                             | &check;      |
| allowParticipantsChatWith               | Int                                 | &check;      |
| allowParticipantsToRename               | Boolean                             | &check;      |
| allowShowZoomWindows                    | Boolean                             | &check;      |
| allowUsersSaveChats                     | Int                                 | &check;      |
| allowUsersToDeleteMessagesInMeetingChat | Boolean                             | &check;      |
| annotation                              | Boolean                             | &check;      |
| anonymousQuestionAnswer                 | Boolean                             | &check;      |
| attentionModeFocusMode                  | Boolean                             | &check;      |
| autoAnswer                              | Boolean                             | &check;      |
| autoSavingChat                          | Boolean                             | &check;      |
| breakoutRoom                            | Boolean                             | &check;      |
| breakoutRoomSchedule                    | Boolean                             | &check;      |
| chat                                    | Boolean                             | &check;      |
| closedCaption                           | Boolean                             | &check;      |
| closedCaptioning                        | Map<String,Boolean>                 | &check;      |
| coHost                                  | Boolean                             | &check;      |
| customDataCenterRegions                 | Boolean                             | &check;      |
| customLiveStreamingService              | Boolean                             | &check;      |
| customServiceInstructions               | String                              | &check;      |
| dataCenterRegions                       | List<String>                        | &check;      |
| disableScreenSharingForHostMeetings     | Boolean                             | &check;      |
| disableScreenSharingForInMeetingGuests  | Boolean                             | &check;      |
| dscpAudio                               | Int                                 | &check;      |
| dscpDual                                | Boolean                             | &check;      |
| dscpMarking                             | Boolean                             | &check;      |
| dscpVideo                               | Int                                 | &check;      |
| e2eEncryption                           | Boolean                             | &check;      |
| entryExitChime                          | String                              | &check;      |
| farEndCameraControl                     | Boolean                             | &check;      |
| feedback                                | Boolean                             | &check;      |
| fileTransfer                            | Boolean                             | &check;      |
| groupHd                                 | Boolean                             | &check;      |
| joinFromDesktop                         | Boolean                             | &check;      |
| joinFromMobile                          | Boolean                             | &check;      |
| languageInterpretation                  | InMeeting.LanguageInterpretation    | &check;      |
| manualCaptioning                        | Map<String,Boolean>                 | &check;      |
| meetingPolling                          | Map<String,Boolean>                 | &check;      |
| meetingReactions                        | Boolean                             | &check;      |
| meetingReactionsEmojis                  | String                              | &check;      |
| meetingSurvey                           | Boolean                             | &check;      |
| nonVerbalFeedback                       | Boolean                             | &check;      |
| originalAudio                           | Boolean                             | &check;      |
| p2pConnection                           | Boolean                             | &check;      |
| p2pPorts                                | Boolean                             | &check;      |
| participantsShareSimultaneously         | String                              | &check;      |
| polling                                 | Boolean                             | &check;      |
| portsRange                              | String                              | &check;      |
| postMeetingFeedback                     | Boolean                             | &check;      |
| privateChat                             | Boolean                             | &check;      |
| recordPlayOwnVoice                      | Boolean                             | &check;      |
| remoteControl                           | Boolean                             | &check;      |
| remoteSupport                           | Boolean                             | &check;      |
| requestPermissionToUnmuteParticipants   | Boolean                             | &check;      |
| screenSharing                           | Boolean                             | &check;      |
| sendingDefaultEmailInvites              | Boolean                             | &check;      |
| showAJoinFromYourBrowserLink            | Boolean                             | &check;      |
| showMeetingControlToolbar               | Boolean                             | &check;      |
| slideControl                            | Boolean                             | &check;      |
| stereoAudio                             | Boolean                             | &check;      |
| uncheckedDataCenterRegions              | List<String>                        | &check;      |
| useHtmlFormatEmail                      | Boolean                             | &check;      |
| virtualBackground                       | Boolean                             | &check;      |
| virtualBackgroundSettings               | InMeeting.VirtualBackgroundSettings | &check;      |
| watermark                               | Boolean                             | &check;      |
| webinarChat                             | InMeeting.WebinarChat               | &check;      |
| webinarLiveStreaming                    | InMeeting.WebinarLiveStreaming      | &check;      |
| webinarPolling                          | Map<String,Boolean>                 | &check;      |
| webinarQuestionAnswer                   | Boolean                             | &check;      |
| webinarReactions                        | Boolean                             | &check;      |
| webinarSurvey                           | Boolean                             | &check;      |
| whiteboard                              | Boolean                             | &check;      |
| whoCanShareScreen                       | String                              | &check;      |
| whoCanShareScreenWhenSomeoneIsSharing   | String                              | &check;      |

#### InMeeting.LanguageInterpretation
| **Name**                                         | **Type**     | **Nullable** |
| ------------------------------------------------ | ------------ | ------------ |
| allowParticipantsToSpeakInListeningChannel       | Boolean      | &check;      |
| allowUpTo25CustomLanguagesWhenSchedulingMeetings | Boolean      | &check;      |
| customLanguages                                  | List<String> | &check;      |
| enable                                           | Boolean      | &check;      |
| enableLanguageInterpretationByDefault            | Boolean      | &check;      |
| languages                                        | List<String> | &check;      |

#### InMeeting.VirtualBackgroundSettings
| **Name**          | **Type**                                       | **Nullable** |
| ----------------- | ---------------------------------------------- | ------------ |
| allowUploadCustom | Boolean                                        | &check;      |
| allowVideos       | Boolean                                        | &check;      |
| enable            | Boolean                                        | &check;      |
| files             | List<InMeeting.VirtualBackgroundSettings.File> | &check;      |

#### InMeeting.VirtualBackgroundSettings.File
| **Name**  | **Type** | **Nullable** |
| --------- | -------- | ------------ |
| id        | String   | &check;      |
| isDefault | Boolean  | &check;      |
| name      | String   | &check;      |
| size      | Int      | &check;      |
| type      | String   | &check;      |

#### InMeeting.WebinarChat
| **Name**                        | **Type** | **Nullable** |
| ------------------------------- | -------- | ------------ |
| allowAttendeesChatWith          | Int      | &check;      |
| allowAutoSaveLocalChatFile      | Boolean  | &check;      |
| allowPanelistsChatWith          | Int      | &check;      |
| allowPanelistsSendDirectMessage | Boolean  | &check;      |
| allowUsersSaveChats             | Int      | &check;      |
| defaultAttendeesChatWith        | Int      | &check;      |
| enable                          | Boolean  | &check;      |

#### InMeeting.WebinarLiveStreaming
| **Name**                  | **Type**     | **Nullable** |
| ------------------------- | ------------ | ------------ |
| customServiceInstructions | String       | &check;      |
| enable                    | Boolean      | &check;      |
| liveStreamingReminder     | Boolean      | &check;      |
| liveStreamingService      | List<String> | &check;      |

#### MeetingAuthenticationSettings
| **Name**                     | **Type**                                                  | **Nullable** |
| ---------------------------- | --------------------------------------------------------- | ------------ |
| allowAuthenticationException | Boolean                                                   | &check;      |
| authenticationOptions        | List<MeetingAuthenticationSettings.AuthenticationOptions> | &check;      |
| meetingAuthentication        | Boolean                                                   | &check;      |

#### MeetingAuthenticationSettings.AuthenticationOptions
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| defaultOption | Boolean  | &check;      |
| domains       | String   | &check;      |
| id            | String   | &check;      |
| name          | String   | &check;      |
| type          | String   | &check;      |
| visible       | Boolean  | &check;      |

#### MeetingSecuritySettings
| **Name**                              | **Type**                                           | **Nullable** |
| ------------------------------------- | -------------------------------------------------- | ------------ |
| autoSecurity                          | Boolean                                            | &check;      |
| blockUserDomain                       | Boolean                                            | &check;      |
| blockUserDomainList                   | List<String>                                       | &check;      |
| embedPasswordInJoinLink               | Boolean                                            | &check;      |
| encryptionType                        | String                                             | &check;      |
| endToEndEncryptedMeetings             | Boolean                                            | &check;      |
| meetingPassword                       | Boolean                                            | &check;      |
| meetingPasswordRequirement            | MeetingSecuritySettings.MeetingPasswordRequirement | &check;      |
| onlyAuthenticatedCanJoinFromWebclient | Boolean                                            | &check;      |
| phonePassword                         | Boolean                                            | &check;      |
| pmiPassword                           | Boolean                                            | &check;      |
| requirePasswordForScheduledMeeting    | Boolean                                            | &check;      |
| requirePasswordForScheduledWebinar    | Boolean                                            | &check;      |
| waitingRoom                           | Boolean                                            | &check;      |
| waitingRoomSettings                   | MeetingSecuritySettings.WaitingRoomSettings        | &check;      |
| webinarPassword                       | Boolean                                            | &check;      |

#### MeetingSecuritySettings.MeetingPasswordRequirement
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

#### MeetingSecuritySettings.WaitingRoomSettings
| **Name**                                    | **Type** | **Nullable** |
| ------------------------------------------- | -------- | ------------ |
| participantsToPlaceInWaitingRoom            | Int      | &check;      |
| usersWhoCanAdmitParticipantsFromWaitingRoom | Int      | &check;      |
| whitelistedDomainsForWaitingRoom            | Int      | &check;      |

#### OtherOptions
| **Name**                          | **Type**            | **Nullable** |
| --------------------------------- | ------------------- | ------------ |
| allowAutoActiveUsers              | Boolean             | &check;      |
| allowUsersContactSupportViaChat   | Boolean             | &check;      |
| allowUsersEnterAndSharePronouns   | Boolean             | &check;      |
| blurSnapshot                      | Boolean             | &check;      |
| displayMeetingsScheduledForOthers | Boolean             | &check;      |
| meetingQosAndMos                  | Int                 | &check;      |
| showOneUserMeetingOnDashboard     | Boolean             | &check;      |
| useCdn                            | String              | &check;      |
| webinarRegistrationOptions        | Map<String,Boolean> | &check;      |

#### PasswordRequirement
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| consecutiveCharactersLength | Int      | &check;      |
| haveSpecialCharacter        | Boolean  | &check;      |
| minimumPasswordLength       | Int      | &check;      |
| weakEnhanceDetection        | Boolean  | &check;      |

#### Profile
| **Name**                 | **Type**                         | **Nullable** |
| ------------------------ | -------------------------------- | ------------ |
| recordingStorageLocation | Profile.RecordingStorageLocation | &check;      |

#### Profile.RecordingStorageLocation
| **Name**      | **Type**     | **Nullable** |
| ------------- | ------------ | ------------ |
| allowedValues | List<String> | &check;      |
| value         | String       | &check;      |

#### Recording
| **Name**                                   | **Type**                               | **Nullable** |
| ------------------------------------------ | -------------------------------------- | ------------ |
| accountUserAccessRecording                 | Boolean                                | &check;      |
| allowRecoveryDeletedCloudRecordings        | Boolean                                | &check;      |
| archive                                    | Recording.Archive                      | &check;      |
| autoDeleteCmr                              | Boolean                                | &check;      |
| autoDeleteCmrDays                          | Int                                    | &check;      |
| autoRecording                              | String                                 | &check;      |
| cloudRecording                             | Boolean                                | &check;      |
| cloudRecordingDownload                     | Boolean                                | &check;      |
| cloudRecordingDownloadHost                 | Boolean                                | &check;      |
| displayParticipantName                     | Boolean                                | &check;      |
| hostDeleteCloudRecording                   | Boolean                                | &check;      |
| ipAddressAccessControl                     | Recording.IpAddressAccessControl       | &check;      |
| localRecording                             | Boolean                                | &check;      |
| optimizeRecordingFor3rdPartyVideoEditor    | Boolean                                | &check;      |
| preventHostAccessRecording                 | Boolean                                | &check;      |
| recordAudioFile                            | Boolean                                | &check;      |
| recordFilesSeparately                      | Map<String,Boolean>                    | &check;      |
| recordGalleryView                          | Boolean                                | &check;      |
| recordSpeakerView                          | Boolean                                | &check;      |
| recordingAudioTranscript                   | Boolean                                | &check;      |
| recordingDisclaimer                        | Boolean                                | &check;      |
| recordingPasswordRequirement               | Recording.RecordingPasswordRequirement | &check;      |
| recordingThumbnails                        | Boolean                                | &check;      |
| requiredPasswordForExistingCloudRecordings | Boolean                                | &check;      |
| requiredPasswordForSharedCloudRecordings   | Boolean                                | &check;      |
| saveChatText                               | Boolean                                | &check;      |
| saveCloseCaption                           | Boolean                                | &check;      |
| savePanelistChat                           | Boolean                                | &check;      |
| savePollResults                            | Boolean                                | &check;      |
| showTimestamp                              | Boolean                                | &check;      |
| smartRecording                             | Map<String,Boolean>                    | &check;      |

#### Recording.Archive
| **Name** | **Type**                   | **Nullable** |
| -------- | -------------------------- | ------------ |
| enable   | Boolean                    | &check;      |
| settings | Recording.Archive.Settings | &check;      |
| type     | Int                        | &check;      |

#### Recording.Archive.Settings
| **Name**                           | **Type** | **Nullable** |
| ---------------------------------- | -------- | ------------ |
| actionWhenArchiveFailed            | Int      | &check;      |
| archiveRetention                   | Int      | &check;      |
| audioFile                          | Boolean  | &check;      |
| ccTranscriptFile                   | Boolean  | &check;      |
| chatFile                           | Boolean  | &check;      |
| chatWithDirectMessage              | Boolean  | &check;      |
| chatWithSenderEmail                | Boolean  | &check;      |
| notificationWhenArchivingStarts    | Int      | &check;      |
| playVoicePromptWhenArchivingStarts | Int      | &check;      |
| videoFile                          | Boolean  | &check;      |

#### Recording.IpAddressAccessControl
| **Name**            | **Type** | **Nullable** |
| ------------------- | -------- | ------------ |
| enable              | Boolean  | &check;      |
| ipAddressesOrRanges | String   | &check;      |

#### Recording.RecordingPasswordRequirement
| **Name**             | **Type** | **Nullable** |
| -------------------- | -------- | ------------ |
| haveLetter           | Boolean  | &check;      |
| haveNumber           | Boolean  | &check;      |
| haveSpecialCharacter | Boolean  | &check;      |
| length               | Int      | &check;      |
| onlyAllowNumeric     | Boolean  | &check;      |

#### RecordingAuthenticationSettings
| **Name**                | **Type**                                                    | **Nullable** |
| ----------------------- | ----------------------------------------------------------- | ------------ |
| authenticationOptions   | List<RecordingAuthenticationSettings.AuthenticationOptions> | &check;      |
| recordingAuthentication | Boolean                                                     | &check;      |

#### RecordingAuthenticationSettings.AuthenticationOptions
| **Name**      | **Type** | **Nullable** |
| ------------- | -------- | ------------ |
| defaultOption | Boolean  | &check;      |
| domains       | String   | &check;      |
| id            | String   | &check;      |
| name          | String   | &check;      |
| type          | String   | &check;      |
| visible       | Boolean  | &check;      |

#### ScheduleMeeting
| **Name**                                | **Type**                                   | **Nullable** |
| --------------------------------------- | ------------------------------------------ | ------------ |
| alwaysDisplayZoomMeetingAsTopic         | Map<String,Boolean>                        | &check;      |
| alwaysDisplayZoomWebinarAsTopic         | Map<String,Boolean>                        | &check;      |
| audioType                               | String                                     | &check;      |
| enforceLogin                            | Boolean                                    | &check;      |
| enforceLoginDomains                     | String                                     | &check;      |
| enforceLoginWithDomains                 | Boolean                                    | &check;      |
| forcePmiJbhPassword                     | Boolean                                    | &check;      |
| hideMeetingDescription                  | Map<String,Boolean>                        | &check;      |
| hideWebinarDescription                  | Map<String,Boolean>                        | &check;      |
| hostVideo                               | Boolean                                    | &check;      |
| jbhTime                                 | Int                                        | &check;      |
| joinBeforeHost                          | Boolean                                    | &check;      |
| meetingPasswordRequirement              | ScheduleMeeting.MeetingPasswordRequirement | &check;      |
| notStoreMeetingTopic                    | Boolean                                    | &check;      |
| participantVideo                        | Boolean                                    | &check;      |
| personalMeeting                         | Boolean                                    | &check;      |
| requirePasswordForInstantMeetings       | Boolean                                    | &check;      |
| requirePasswordForPmiMeetings           | String                                     | &check;      |
| requirePasswordForScheduledMeetings     | Boolean                                    | &check;      |
| requirePasswordForSchedulingNewMeetings | Boolean                                    | &check;      |
| usePmiForInstantMeetings                | Boolean                                    | &check;      |
| usePmiForScheduledMeetings              | Boolean                                    | &check;      |

#### ScheduleMeeting.MeetingPasswordRequirement
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

#### Security
| **Name**                             | **Type**            | **Nullable** |
| ------------------------------------ | ------------------- | ------------ |
| adminChangeUserInfo                  | Boolean             | &check;      |
| hideBillingInfo                      | Boolean             | &check;      |
| importPhotosFromDevices              | Boolean             | &check;      |
| passwordRequirement                  | PasswordRequirement | &check;      |
| signAgainPeriodForInactivityOnClient | Int                 | &check;      |
| signAgainPeriodForInactivityOnWeb    | Int                 | &check;      |
| signInWithTwoFactorAuth              | String              | &check;      |
| signInWithTwoFactorAuthGroups        | List<String>        | &check;      |
| signInWithTwoFactorAuthRoles         | List<String>        | &check;      |
| userModifiableInfoByAdmin            | List<String>        | &check;      |

#### Telephony
| **Name**            | **Type**                   | **Nullable** |
| ------------------- | -------------------------- | ------------ |
| audioConferenceInfo | String                     | &check;      |
| telephonyRegions    | Telephony.TelephonyRegions | &check;      |
| thirdPartyAudio     | String                     | &check;      |

#### Telephony.TelephonyRegions
| **Name**        | **Type**     | **Nullable** |
| --------------- | ------------ | ------------ |
| allowedValues   | List<String> | &check;      |
| selectionValues | String       | &check;      |

#### Tsp
| **Name**                     | **Type**     | **Nullable** |
| ---------------------------- | ------------ | ------------ |
| callOut                      | Boolean      | &check;      |
| callOutCountries             | List<String> | &check;      |
| displayTollFreeNumbers       | Boolean      | &check;      |
| showInternationalNumbersLink | Boolean      | &check;      |
