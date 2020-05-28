{
  "name": "propozycja",
  "permissions": "NONE",
  "restriction": "1",
  "_id": "BqzYz",
  "actions": [
    {
      "info": "1",
      "find": "propozycje",
      "storage": "1",
      "varName": "kanal",
      "name": "Find Channel"
    },
    {
      "member": "1",
      "varName": "",
      "info": "7",
      "storage": "1",
      "varName2": "user_tag",
      "name": "Store Member Things"
    },
    {
      "member": "1",
      "varName": "",
      "info": "16",
      "storage": "1",
      "varName2": "avatar_URL",
      "name": "Store Member Info"
    },
    {
      "info": "1",
      "infoIndex": "1",
      "storage": "1",
      "varName": "propozycja_tresc",
      "name": "Store Command Params"
    },
    {
      "condition": "0",
      "comparison": "1",
      "value": "1",
      "iftrue": "0",
      "iftrueVal": "",
      "iffalse": "3",
      "iffalseVal": "4",
      "name": "Check Parameters"
    },
    {
      "title": "",
      "author": "",
      "color": "",
      "timestamp": "false",
      "url": "",
      "authorIcon": "",
      "imageUrl": "",
      "thumbUrl": "",
      "storage": "1",
      "varName": "embed_blad",
      "name": "Create Embed Message"
    },
    {
      "storage": "1",
      "varName": "embed_blad",
      "message": "**Błąd:** Napisz swoją propozycję!",
      "name": "Set Embed Description"
    },
    {
      "storage": "1",
      "varName": "embed_blad",
      "channel": "0",
      "varName2": "",
      "storage3": "0",
      "varName3": "",
      "name": "Send Embed Message"
    },
    {
      "name": "End Action Sequence"
    },
    {
      "title": "",
      "author": "${tempVars(\"user_tag\")}",
      "color": "#69ff84 ",
      "timestamp": "false",
      "url": "",
      "authorIcon": "${tempVars(\"avatar_URL\")}",
      "imageUrl": "",
      "thumbUrl": "",
      "storage": "1",
      "varName": "propozycja_embed",
      "name": "Create Embed Message"
    },
    {
      "storage": "1",
      "varName": "propozycja_embed",
      "message": "${tempVars(\"propozycja_tresc\")}",
      "name": "Set Embed Description"
    },
    {
      "storage": "1",
      "varName": "propozycja_embed",
      "message": "✅ Jestem za! • ❌ Jestem przeciw!",
      "footerIcon": "",
      "name": "Set Embed Footer"
    },
    {
      "storage": "1",
      "varName": "propozycja_embed",
      "channel": "5",
      "varName2": "kanal",
      "storage3": "1",
      "varName3": "wiadomosc_sended",
      "name": "Send Embed Message"
    },
    {
      "storage": "1",
      "varName": "wiadomosc_sended",
      "emoji": "4",
      "varName2": "✅",
      "varName3": "",
      "name": "Add Reaction"
    },
    {
      "storage": "1",
      "varName": "wiadomosc_sended",
      "emoji": "4",
      "varName2": "❌",
      "varName3": "",
      "name": "Add Reaction"
    },
    {
      "time": "2",
      "measurement": "1",
      "name": "Wait"
    },
    {
      "storage": "0",
      "varName": "",
      "name": "Delete Message"
    }
  ]
}
