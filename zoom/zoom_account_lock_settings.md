---
description: Zoom Account Lock Settings
---
zoom_account_lock_settings
--------------------------

| **Name**                | **Type**                | **Nullable** |
| ----------------------- | ----------------------- | ------------ |
| audioConferencing       | AudioConferencing       | &check;      |
| emailNotification       | Map<String,Boolean>     | &check;      |
| inMeeting               | InMeeting               | &check;      |
| meetingSecuritySettings | MeetingSecuritySettings | &check;      |
| otherOptions            | OtherOptions            | &check;      |
| recording               | Recording               | &check;      |
| scheduleMeeting         | ScheduleMeeting         | &check;      |
| telephony               | Telephony               | &check;      |
| tsp                     | Tsp                     | &check;      |

#### AudioConferencing
| **Name**                    | **Type** | **Nullable** |
| --------------------------- | -------- | ------------ |
| tollFreeAndFeeBasedTollCall | Boolean  | &check;      |

#### InMeeting
| **Name**                                | **Type** | **Nullable** |
| --------------------------------------- | -------- | ------------ |
| alertGuestJoin                          | Boolean  | &check;      |
| allowHostToEnableFocusMode              | Boolean  | &check;      |
| allowLiveStreaming                      | Boolean  | &check;      |
| allowShowZoomWindows                    | Boolean  | &check;      |
| allowUsersToDeleteMessagesInMeetingChat | Boolean  | &check;      |
| annotation                              | Boolean  | &check;      |
| anonymousQuestionAnswer                 | Boolean  | &check;      |
| attentionModeFocusMode                  | Boolean  | &check;      |
| autoAnswer                              | Boolean  | &check;      |
| autoSavingChat                          | Boolean  | &check;      |
| breakoutRoom                            | Boolean  | &check;      |
| chat                                    | Boolean  | &check;      |
| closedCaption                           | Boolean  | &check;      |
| coHost                                  | Boolean  | &check;      |
| customDataCenterRegions                 | Boolean  | &check;      |
| disableScreenSharingForHostMeetings     | Boolean  | &check;      |
| disableScreenSharingForInMeetingGuests  | Boolean  | &check;      |
| dscpMarking                             | Boolean  | &check;      |
| e2eEncryption                           | Boolean  | &check;      |
| entryExitChime                          | String   | &check;      |
| farEndCameraControl                     | Boolean  | &check;      |
| feedback                                | Boolean  | &check;      |
| fileTransfer                            | Boolean  | &check;      |
| groupHd                                 | Boolean  | &check;      |
| languageInterpretation                  | Boolean  | &check;      |
| manualCaptions                          | Boolean  | &check;      |
| meetingReactions                        | Boolean  | &check;      |
| meetingSurvey                           | Boolean  | &check;      |
| nonVerbalFeedback                       | Boolean  | &check;      |
| originalAudio                           | Boolean  | &check;      |
| polling                                 | Boolean  | &check;      |
| postMeetingFeedback                     | Boolean  | &check;      |
| privateChat                             | Boolean  | &check;      |
| remoteControl                           | Boolean  | &check;      |
| remoteSupport                           | Boolean  | &check;      |
| requestPermissionToUnmuteParticipants   | Boolean  | &check;      |
| saveCaption                             | Boolean  | &check;      |
| saveCaptions                            | Boolean  | &check;      |
| screenSharing                           | Boolean  | &check;      |
| sendingDefaultEmailInvites              | Boolean  | &check;      |
| showMeetingControlToolbar               | Boolean  | &check;      |
| slideControl                            | Boolean  | &check;      |
| stereoAudio                             | Boolean  | &check;      |
| useHtmlFormatEmail                      | Boolean  | &check;      |
| virtualBackground                       | Boolean  | &check;      |
| webinarChat                             | Boolean  | &check;      |
| webinarLiveStreaming                    | Boolean  | &check;      |
| webinarPolling                          | Boolean  | &check;      |
| webinarQuestionAnswer                   | Boolean  | &check;      |
| webinarReactions                        | Boolean  | &check;      |
| webinarSurvey                           | Boolean  | &check;      |
| whiteboard                              | Boolean  | &check;      |

#### MeetingSecuritySettings
| **Name**                              | **Type** | **Nullable** |
| ------------------------------------- | -------- | ------------ |
| approvedOrDeniedCountriesOrRegions    | Boolean  | &check;      |
| autoSecurity                          | Boolean  | &check;      |
| blockUserDomain                       | Boolean  | &check;      |
| chatEtiquetteTool                     | Boolean  | &check;      |
| embedPasswordInJoinLink               | Boolean  | &check;      |
| encryptionType                        | Boolean  | &check;      |
| endToEndEncryptedMeetings             | Boolean  | &check;      |
| meetingPassword                       | Boolean  | &check;      |
| onlyAuthenticatedCanJoinFromWebclient | Boolean  | &check;      |
| phonePassword                         | Boolean  | &check;      |
| pmiPassword                           | Boolean  | &check;      |
| waitingRoom                           | Boolean  | &check;      |
| webinarPassword                       | Boolean  | &check;      |

#### OtherOptions
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| blurSnapshot               | Boolean  | &check;      |
| webinarRegistrationOptions | Boolean  | &check;      |

#### Recording
| **Name**                   | **Type** | **Nullable** |
| -------------------------- | -------- | ------------ |
| accountUserAccessRecording | Boolean  | &check;      |
| archive                    | Boolean  | &check;      |
| autoDeleteCmr              | Boolean  | &check;      |
| autoRecording              | Boolean  | &check;      |
| cloudRecording             | Boolean  | &check;      |
| cloudRecordingDownload     | Boolean  | &check;      |
| hostDeleteCloudRecording   | Boolean  | &check;      |
| ipAddressAccessControl     | Boolean  | &check;      |
| localRecording             | Boolean  | &check;      |
| preventHostAccessRecording | Boolean  | &check;      |
| recordingAuthentication    | Boolean  | &check;      |

#### ScheduleMeeting
| **Name**                                | **Type** | **Nullable** |
| --------------------------------------- | -------- | ------------ |
| alwaysDisplayZoomMeetingAsTopic         | Boolean  | &check;      |
| audioType                               | Boolean  | &check;      |
| embedPasswordInJoinLink                 | Boolean  | &check;      |
| enforceLogin                            | Boolean  | &check;      |
| enforceLoginDomains                     | String   | &check;      |
| enforceLoginWithDomains                 | Boolean  | &check;      |
| hostVideo                               | Boolean  | &check;      |
| joinBeforeHost                          | Boolean  | &check;      |
| meetingAuthentication                   | Boolean  | &check;      |
| notStoreMeetingTopic                    | Boolean  | &check;      |
| participantVideo                        | Boolean  | &check;      |
| requirePasswordForInstantMeetings       | Boolean  | &check;      |
| requirePasswordForPmiMeetings           | Boolean  | &check;      |
| requirePasswordForSchedulingNewMeetings | Boolean  | &check;      |
| usePmiForInstantMeetings                | Boolean  | &check;      |
| usePmiForScheduledMeetings              | Boolean  | &check;      |

#### Telephony
| **Name**         | **Type** | **Nullable** |
| ---------------- | -------- | ------------ |
| telephonyRegions | Boolean  | &check;      |
| thirdPartyAudio  | Boolean  | &check;      |

#### Tsp
| **Name**                     | **Type** | **Nullable** |
| ---------------------------- | -------- | ------------ |
| callOut                      | Boolean  | &check;      |
| showInternationalNumbersLink | Boolean  | &check;      |
