# WhatsApp-Web-API-
WhatsApp Web functions

Here are just some functions you can call to get certain information from phone numbers that are connected to WhatsApp.
You need to connect to WhatsApp Web in order to use any of the functions below.

Replace ```*phone number*``` with your phone number or any other phone number



**-Profile Pictures:**

```var nr = *phone number*; Store.ProfilePicThumb.find(nr+ '@c.us').then(function(r){ console.log(r)})```

**-Online/Offline:**

```var nr = *phone number*; Store.Presence.find(nr+ '@c.us').then(function(r){ console.log(r)}) ```

**-Status:**

```var nr = *phone number*; Store.Status._find(nr+ '@c.us').then(function(r){ console.log(r)}) ```

**-Online Counter**

```var nr = *phone number*; Store.Wap.lastseenFind(nr+ '@c.us').then(function(r){ console.log(r)}) //counting when target is online```

**-List All Groups:**

```var nr = *phone number*; Store.Wap.commonGroupsFind(nr+ '@c.us').then(function(r){ console.log(r)}) //Amount of groups stored in an Array```


**-Unknown:**

```
var nr = *phone number*; Store.Wap.contactFindQuery(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.MsgInfo.find(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Chat.find(nr+ '@c.us').then(function(r){ console.log(r)}) //Name is stored there
var nr = *phone number*; Store.Props.fetch(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Chat._find(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Wap.groupMetadataFindFromPhone(nr+ '@c.us').then(function(r){ console.log(r)}) //useless "ok" ?!
var nr = *phone number*; Store.Msg.getContext(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Msg.getStarred(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Msg.queryMedia(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Msg.resyncChatMsgs(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Msg.resyncReceipts(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Msg.search(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Msg.send(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Msg._findQuery(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Msg._hasSynced(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Msg._search(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Msg.findQuery(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Msg(nr+ '@c.us').then(function(r){ console.log(r)})
```

**-All "Wap" functions**
```-acceptGroupInvite:ƒ (e)
-addContact:ƒ ()
-addParticipant:ƒ ()
-changeSubject:ƒ ()
-chatFindQuery:ƒ ()
-clearBPQueue:ƒ ()
-commonGroupsFind:ƒ (e)
-contactFindBroadcast:ƒ (e)
-contactFindQuery:ƒ ()
-createGroup:ƒ ()
-delete:ƒ ()
-deletePicture:ƒ ()
-downloadImage:ƒ (e)
-error2412:ƒ ()
-getCapabilities:ƒ (e)
-getPlaintextMediaInfo:ƒ (e)
-getStatusPrivacy:ƒ ()
-groupInviteCode:ƒ (e)
-groupInviteInfo:ƒ (e)
-groupMetadataFind:ƒ (e)
-groupMetadataFindFromPhone:ƒ ()
-handle:ƒ ()
-lastseenFind:ƒ (e)
-leaveGroup:ƒ ()
-logoutToken:ƒ ()
-msgCreateRecord:ƒ ()
-msgFindQuery:ƒ ()
-presenceSubscribe:ƒ (e)
-profilePicFind:ƒ (e)
-profilePicFindThumbFromPhone:ƒ (e,t)
-promoteParticipant:ƒ ()
-pushToken:ƒ (e)
-queryBusinessProfile:ƒ (e)
-queryExist:ƒ (e)
-queryIdentity:ƒ ()
-queryLinkPreview:ƒ ()
-queryMsgInfo:ƒ ()
-queryReceivedActions:ƒ ()
-queryServerProps:ƒ ()
-queryVCard:ƒ ()
-recentEmojiQuery:ƒ ()
-removeParticipant:ƒ ()
-requestDeviceUploadLogs:ƒ ()
-requestEncryptedMediaUpload:ƒ (e,t)
-requestMediaReupload:ƒ ()
-requestMediaUpload:ƒ (e,t,n)
-resyncMessages:ƒ ()
-resyncPictures:ƒ (e)
-resyncReceipts:ƒ ()
-revokeGroupInvite:ƒ (e)
-sendChatstateComposing:ƒ (e)
-sendChatstatePaused:ƒ (e)
-sendChatstateRecording:ƒ (e)
-sendConversationArchive:ƒ ()
-sendConversationClear:ƒ ()
-sendConversationDelete:ƒ ()
-sendConversationMute:ƒ ()
-sendConversationNotSpam:ƒ ()
-sendConversationPin:ƒ ()
-sendConversationSeen:ƒ ()
-sendConversationUnseen:ƒ ()
-sendMedia:ƒ ()
-sendMessageDelete:ƒ ()
-sendMessagePlayed:ƒ ()
-sendMessageStarred:ƒ ()
-sendPing:ƒ (e)
-sendPresenceAvailable:ƒ ()
-sendPresenceUnavailable:ƒ ()
-sendSetBlock:ƒ ()
-sendSetPicture:ƒ ()
-sendSetStatus:ƒ ()
-sendSpamReport:ƒ ()
-sendStatusSeen:ƒ ()
-sendUnstarAll:ƒ ()
-setPushname:ƒ ()
-setRememberMe:ƒ (e)
-setSharedSecret:ƒ ()
-setStatusPrivacy:ƒ ()
-setVersion:ƒ (e,t)
-statusFind:ƒ (e)
-statusQuery:ƒ ()
-__proto__:Object```
