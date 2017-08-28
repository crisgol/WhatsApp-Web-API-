# WhatsApp-Web-API-
WhatsApp Web functions

Here are just some functions you can call to get certain information from phone numbers that are connected to WhatsApp.
You need to connect to WhatsApp Web in order to use any of the functions below.


-Profile Pictures:

```var nr = *phone number*; Store.ProfilePicThumb.find(nr+ '@c.us').then(function(r){ console.log(r)})```

-Online/Offline:

```var nr = *phone number*; Store.Presence.find(nr+ '@c.us').then(function(r){ console.log(r)}) ```

-Status:

```var nr = *phone number*; Store.Status._find(nr+ '@c.us').then(function(r){ console.log(r)}) ```

-Online Counter

```var nr = *phone number*; Store.Wap.lastseenFind(nr+ '@c.us').then(function(r){ console.log(r)}) //counting when target is online```

-List All Groups:

```var nr = *phone number*; Store.Wap.commonGroupsFind(nr+ '@c.us').then(function(r){ console.log(r)}) //Amount of groups stored in an Array```


-Unknown:

```var nr = *phone number*; Store.MsgInfo.find(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Chat.find(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Props.fetch(nr+ '@c.us').then(function(r){ console.log(r)})
var nr = *phone number*; Store.Wap.groupMetadataFindFromPhone(nr+ '@c.us').then(function(r){ console.log(r)}) //useless "ok" ?!```
