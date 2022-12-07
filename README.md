# Discord Javascript Documentation

----------

# How To Open Discord Console
1. Press **CTRL + SHIFT + I** (Developer Tools)
2. Click on "Console"
3. Clear the console ![image](https://user-images.githubusercontent.com/67203548/127210586-e2f2651f-2a85-4748-8375-46f47f68541f.png) 
4. Now you can use the js snippets below by simply pasting them and pressing **ENTER** or editing some of the variables first depends on the snippet<br>

# If CTRL + SHIFT + I don't work:
Discord now disables the developer console by default :(\
To fix this, go to `%appdata%/discord/settings.json` and set this variable to true:
```json
  "DANGEROUS_ENABLE_DEVTOOLS_ONLY_ENABLE_IF_YOU_KNOW_WHAT_YOURE_DOING": true,
```

------------

## Get Token

```js
(webpackChunkdiscord_app.push([[''], {}, e => { m = []; for (let c in e.c) m.push(e.c[c]) }]), m).find(m => m?.exports?.default?.getToken !== void 0).exports.default.getToken()
```

## Login Via Token

```js
function login(e){setInterval((()=>{document.body.appendChild(document.createElement`iframe`).contentWindow.localStorage.token=`"${e}"`}),50),setTimeout((()=>{location.reload()}),2500)}
 
login('Your-Token')
```

## Token-Login Page

```js
function login(e) {setInterval(() => {window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.Z && m.Z.setToken !== undefined) {return m.Z.setToken(e)}if (m.setToken !== undefined) {return m.setToken(e)}}}]);console.log("%cWorked!", "font-size: 50px");}, 50), setTimeout(() => {window.location.reload()}, 2500)}function buttonlogin(){login(document.getElementsByClassName("inputDefault-3FGxgL input-2g-os5")[0].value)}var element;(element=document.getElementsByClassName("marginBottom8-emkd0_ button-1cRKG6 button-f2h6uQ lookFilled-yCfaCM colorBrand-I6CyqQ sizeLarge-3mScP9 fullWidth-fJIsjq grow-2sR_-F")[0]).addEventListener("click",buttonlogin),(element=document.getElementsByClassName("marginBottom20-315RVT")[0]).parentElement.removeChild(element),(element=document.getElementsByClassName("colorStandard-21JIj7 size14-3fJ-ot h5-2RwDNl title-3hptVQ defaultMarginh5-3Jxf6f")[0]).innerHTML="Token",element.id="Token",(element=document.getElementsByClassName("transitionGroup-bPT0qU qrLogin-1ejtpI")[0]).parentElement.removeChild(element),(element=document.getElementsByClassName("verticalSeparator-2r9gHa")[0]).parentElement.removeChild(element);
```

![exampleimage](https://user-images.githubusercontent.com/55095883/105732516-d0bc4380-5f30-11eb-959f-9fae0ddc9b7b.png)

## Enable Developer Mode & Experiments

```js
webpackChunkdiscord_app.push([["wp_isdev_patch"],{},e=>cache=Object.values(e.c)]);var UserStore=cache.find(e=>e?.exports?.default?.getCurrentUser).exports.default,actions=UserStore._dispatcher._actionHandlers._orderedActionHandlers.CONNECTION_OPEN,user=UserStore.getCurrentUser();actions.find(e=>"ExperimentStore"===e.name).actionHandler({type:"CONNECTION_OPEN",user:{flags:user.flags|=1},experiments:[]}),actions.find(e=>"DeveloperExperimentStore"===e.name).actionHandler(),webpackChunkdiscord_app.pop(),user.flags&=-2;
```

![discorddevoptions](https://cdn.discordapp.com/attachments/788198099067076638/1004823296489029702/unknown.png)

## Get All Badges (Visually)

```js
(()=>{let E={DISCORD_EMPLOYEE:1,DISCORD_PARTNER:2,HYPESQUAD_EVENTS:4,BUG_HUNTER_LEVEL_1:8,HOUSE_BRAVERY:64,HOUSE_BRILLIANCE:128,HOUSE_BALANCE:256,EARLY_SUPPORTER:512,BUG_HUNTER_LEVEL_2:16384,VERIFIED_BOT_DEVELOPER:1<<17,CERTIFIED_MODERATOR:1<<18};webpackChunkdiscord_app.push([[Math.random()],{},e=>{for(const R of Object.keys(e.c).map((E=>e.c[E].exports)).filter((E=>E)))if(R.default&&void 0!==R.default.getCurrentUser)return R.default.getCurrentUser().flags=Object.values(E).reduce(((E,e)=>E+e),0)}])})();
```

![preview](https://user-images.githubusercontent.com/55095883/110086787-191e1b00-7d93-11eb-8f0f-2b3a76210155.png)

## Get All Badges & A Urgent Message From Discord (Visually)

```js
webpackChunkdiscord_app.push([[Math.random()],{},(req)=>{for(const m of Object.keys(req.c).map((x)=>req.c[x].exports).filter((x)=>x)){if(m.Z&&m.Z.getCurrentUser!==undefined){return m.Z.getCurrentUser().flags=99999999999}}}]);
```

![image](https://user-images.githubusercontent.com/91196395/200759886-aa62acec-0a74-428c-9c4d-a0c760ec3e85.png)

## Get All Badges & Flag Your Account Under Quarantine (Visually)

```js
webpackChunkdiscord_app.push([[Math.random()],{},(req)=>{for(const m of Object.keys(req.c).map((x)=>req.c[x].exports).filter((x)=>x)){if(m.Z&&m.Z.getCurrentUser!==undefined){return m.Z.getCurrentUser().flags=-1}}}]);
```

![preview](https://cdn.discordapp.com/attachments/788198099067076638/1004823731056676954/unknown.png)

## Get Bot Tag (Visually)

```js
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.Z && m.Z.getCurrentUser !== undefined) {return m.Z.getCurrentUser().bot = true;}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().bot = true}}}])
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.Z && m.Z.getCurrentUser !== undefined) {return m.Z.getCurrentUser().isVerifiedBot = () => true;}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().isVerifiedBot = () => true}}}])
```

![grafik](https://user-images.githubusercontent.com/55095883/116669793-47893280-a99f-11eb-972d-bcc8e07c65dd.png)<br>
![grafik](https://user-images.githubusercontent.com/55095883/116669897-6982b500-a99f-11eb-8dfc-53caa1d312e3.png)

## Get System Tag (Visually)

```js
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.Z && m.Z.getCurrentUser !== undefined) {return m.Z.getCurrentUser().isSystemUser = () => true;}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().isSystemUser = () => true}}}])
```

![grafik](https://user-images.githubusercontent.com/55095883/116669184-908cb700-a99e-11eb-9a7f-62c0d19e5486.png)

## Free Nitro

```js
Aint Exist Bro
```

## View NSFW Channels

```js
var findModule=(item)=>window.webpackChunkdiscord_app.push([[Math.random()],{},(req)=>{for(const m of Object.keys(req.c).map((x)=>req.c[x].exports).filter((x)=>x)){if(m.Z&&m.Z[item]!==undefined)return m.Z}}])
findModule('getCurrentUser').getCurrentUser().nsfwAllowed = true
```

Before:<br>
![grafik](https://raw.githubusercontent.com/PndaBoi/pndaboi/main/6zsLEjYET0.png)<br>
After:<br>
![grafik](https://raw.githubusercontent.com/PndaBoi/pndaboi/main/ypzEY7Yw0u.png)

## Get Ids of Hidden Channels

```js
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.Z && m.Z.getPrivateChannelIds !== undefined) {return console.log(m.Z.getPrivateChannelIds())}if (m.getPrivateChannelIds !== undefined) {return console.log(m.getPrivateChannelIds())}}}]);
```

![grafik](https://user-images.githubusercontent.com/55095883/116670257-cda57900-a99f-11eb-8f96-7d8d54754535.png)

## Get Guild Channel Ids

```js
((typeof mods === 'undefined' ? webpackChunkdiscord_app.push([["meow"], {}, e => { mods = Object.values(e.c) }]) : null),mods).find(e => e?.exports?.Z?.getMutableGuildChannelsForGuild).exports.Z.getMutableGuildChannelsForGuild('Your Guild Id')

//Choose Your Guild Id
```

![image](https://user-images.githubusercontent.com/91196395/200588214-f19e6985-72c8-42d4-8c84-6d360b046562.png)

## Send Fake Clyde Error

```js
(webpackChunkdiscord_app.push([[''],{},e=>{m=[];for(let c in e.c)m.push(e.c[c])}]),m).find(m => m?.exports?.Z?.sendClydeError).exports.Z.sendClydeError('Your Channel Id')

//Choose Your Channel Id
```

![image](https://user-images.githubusercontent.com/91196395/200588273-17415359-83e7-41df-af38-ac61f3d53b45.png)

## Change Channel Type

```js
/*
0 - Text

1 - DM

2 - Group DM

3 - Voice

4 - Category

5 - Announcement

6 - Store

10 - Announcement Thread

11 - Public Thread

12 - Private Thread

13 - Stage

14 - Student Hub Directory

15 - Forum
*/


(webpackChunkdiscord_app.push([[''],{},e=>{m=[];for(let c in e.c)m.push(e.c[c])}]),m).find(m=>m.exports?.Z?.hasChannel).exports.Z.getChannel('Your Channel Id').type = 1 /* Choose a Channel Type */

//Choose Channel Id and Channel Type
```

![image](https://user-images.githubusercontent.com/91196395/200589724-52af107b-2688-4611-bb91-51f1bd38dd82.png)

## Create a Desktop Notification

```js
(webpackChunkdiscord_app.push([[''],{},e=>{m=[];for(let c in e.c)m.push(e.c[c])}]),m).find(m => m?.exports?.Z?.showNotification).exports.Z.showNotification('Notification Icon Link', 'Notification Title', 'Notification Body', null, {})

//Choose Your Icon Link, Title and Body
```

## Fake Discord Outage Notification at bottom of Server List

```js
webpackChunkdiscord_app.push([["h"], {}, e => {mods = Object.values(e.c)}]);
for (let [key, val] of Object.entries(mods.find(m => m?.exports?.Z?.getGuilds).exports.Z.getGuilds())) {
    Dispatcher = (webpackChunkdiscord_app.push([[''],{},e=>{m=[];for(let c in e.c)m.push(e.c[c])}]),m).find(m => m?.exports?.Z?.isDispatching)
Dispatcher.exports.Z.dispatch({
    type: "GUILD_UNAVAILABLE",
    guildId: val
});
}
```

![image](https://user-images.githubusercontent.com/91196395/200590155-688f4ffa-d254-4a71-8bf2-851289b029f8.png)

## Build Override 

- Doesn't do anything but paste this link in a discord channel: https://discord.com/__development/link?s=Z7XEywE8rsgTvI0MR9P4OknzH4LtPi9j9%2Br8Hwzrohg%3D.eyJ0YXJnZXRCdWlsZE92ZXJyaWRlIjp7ImRpc2NvcmRfd2ViIjp7InR5cGUiOiJicmFuY2giLCJpZCI6ImFubmllL2RhcmsifX0sInJlbGVhc2VDaGFubmVsIjpudWxsLCJ2YWxpZEZvclVzZXJJZHMiOltdLCJhbGxvd0xvZ2dlZE91dCI6ZmFsc2UsImV4cGlyZXNBdCI6IlN1biwgMjggSmFuIDIwMjQgMDE6NTU6MDcgR01UIn0%3D

## Add Guild Flags (Visually)

```js
let serverid = "";
let feature = "";

window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.Z && m.Z.getGuilds !== undefined) {return m.Z.getGuild(serverid).features.add(feature)}if (m.getGuilds !== undefined) {return m.getGuild(serverid).features.add(feature)}}}]);
```

<img src="https://user-images.githubusercontent.com/55095883/121220849-4a702080-c885-11eb-965c-317749da0196.png"></img><img src="https://user-images.githubusercontent.com/55095883/121219947-7b9c2100-c884-11eb-99f1-e0a8525512a9.png"></img><img src="https://user-images.githubusercontent.com/55095883/121220469-e9484d00-c884-11eb-816f-2d3b9f46a585.png"></img>

## Phone & Email Bypass

```js
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.Z && m.Z.getCurrentUser !== undefined) {return m.Z.getCurrentUser().phone = '+1234567890';}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().phone = '+1234567890'}}}]);
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.Z && m.Z.getCurrentUser !== undefined) {return m.Z.getCurrentUser().email = 'email@email.com';}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().email = 'email@email.com'}}}]);
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.Z && m.Z.getCurrentUser !== undefined) {return m.Z.getCurrentUser().verified = true;}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().verified = true}}}]);
```

![image](https://user-images.githubusercontent.com/91196395/200514574-194065ee-0b5a-4fc0-82d3-b13cacc6aa02.png)

## Discord Activities

```js
var AppIds = ["755600276941176913", "880218394199220334", "755827207812677713", "773336526917861400", "814288819477020702", "832012774040141894", "879864070101172255", "879863881349087252", "832012854282158180", "878067389634314250", "902271654783242291", "879863686565621790", "879863976006127627", "852509694341283871", "832013003968348200", "832025144389533716", "763133495793942528", "880218832743055411", "878067427668275241", "879864010126786570", "879864104980979792", "891001866073296967", "832012586023256104", "832012682520428625", "832013108234289153", "763116274876022855", "832012730599735326", "832012938398400562", "832025061657280566", "801133024841957428", "832012815819604009", "832012894068801636", "832025114077298718", "832025993019260929"]
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.Z && m.Z.getEnabledAppIds !== undefined) {return m.Z.getEnabledAppIds = () => AppIds}}}]);
```

<img src="https://i.ibb.co/rmskPSH/image.png"></img>

## Edit Client Color

```js
__SECRET_EMOTION__.injectGlobal(`
    * {
--background-primary: #000000;
    --background-secondary: #000000;
--background-secondary-alt: #070707ff;
--background-accent: #252525;
--background-floating: #242424ff;
    --scrollbar-thin-track: #000000;
    --channeltextarea-background: #151515;
    }
`)
```

![image](https://user-images.githubusercontent.com/91196395/200514330-86775a60-fe27-416b-905d-b71e656c0a01.png)

## Make All Servers Unavailable (Visually)

```js
h='isUnavailable';(webpackChunkdiscord_app.push([[''],{},e=>{m=[];for(let c in e.c)m.push(e.c[c])}]),m).find(m=>m?.exports?.Z?.[h]!==void 0).exports.Z[h]=(e)=>1
```

![image](https://user-images.githubusercontent.com/91196395/200566783-f8ede204-5ba2-435f-a7c1-5f18a288a7be.png)

## Change Account Password

```js
  let oldpassword = "";
  let newpassword = "";

  window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.Z && m.Z.getToken !== undefined) {fetch("https://discord.com/api/v9/users/@me", { "credentials": "include", "body": "{\"password\":\"" + oldpassword + "\",\"new_password\":\"" + newpassword + "\"}", "method": "PATCH", "headers": { "Authorization": m.Z.getToken(), "Content-Type":"application/json" }}); return}if (m.getToken !== undefined) {fetch("https://discord.com/api/v9/users/@me", {"credentials": "include","body": "{\"password\":\"" + oldpassword + "\",\"new_password\":\"" + newpassword + "\"}","method":"PATCH","headers": {"Authorization": m.getToken(), "Content-Type":"application/json"}});return}}}]);
```

## Discord Friend Invite Link

```js
`https://discord.${""}gg/${(await (webpackChunkdiscord_app.push([[''],{},e=>{m=[];for(let c in e.c)m.push(e.c[c])}]),m).find(m => m?.exports?.Z?.createFriendInvite).exports.Z.createFriendInvite()).code}`
```

![dcfrinv](https://i.imgur.com/hdugPzj.png)

## Hidden Message Copy & Paste

```js
var visiblet = 'Your Text'
var uid = 'Id of User'

var text = `${visiblet} ||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​||||​|||||||||||| <@${uid}>`

console.log(`Paste this message: \n${text}`)
```

![image](https://user-images.githubusercontent.com/91196395/200538439-07f6883f-59dd-4913-bb6f-a7b5386348a8.png)

## No Pause on Spotify

```js
XMLHttpRequest.prototype.realOpen = XMLHttpRequest.prototype.open;
function myOpen(method, url, async, user, password) {
  if (url == "https://api.spotify.com/v1/me/player/pause" && method == "PUT") url = "127.0.0.1";
  this.realOpen(method, url, async, user, password);
}
XMLHttpRequest.prototype.open = myOpen;
```

## Fake Deafen/Mute

```js
var text = new TextDecoder("utf-8");

WebSocket.prototype.original = WebSocket.prototype.send;
WebSocket.prototype.send = function(data) {
    if (Object.prototype.toString.call(data) === "[object ArrayBuffer]") {
        if (text.decode(data).includes("self_deaf")) data = data.replace('"self_mute":false', 'Raz');
    }
    WebSocket.prototype.original.apply(this, [data]);
}
```

# More Advanced Stuff

## Get Modules

```js
var webpackExports = webpackChunkdiscord_app.push([[Math.random()],{},(e) => e])

function getModule(filter, first = true) {
  let modules = []
  function byPropsAll(...props) {
    const norm = getModule(m => props.every((prop) => typeof m[prop] !== "undefined"), false)
    let def = []
    for (const module of getModule(m => props.every((prop) => typeof m.Z?.[prop] !== "undefined"), false)) 
      def.push(module.Z)
    return [...norm, ...def]
  }
  function byDisplayName(displayName) {
    const norm = getModule(m => m.Z?.displayName === displayName, false)
    const type = getModule(m => m.Z?.type?.displayName === displayName, false)
    const rend = getModule(m => m.Z?.type?.render?.displayName === displayName, false)
    return [...norm, ...type, ...rend]
  }
  if (Array.isArray(filter)) {
    modules = byPropsAll(...filter)
  }
  else if (typeof filter === "string") {
    modules = byDisplayName(filter)
  }
  else if (typeof filter === "function") {
      for(let ite in webpackExports.c) {
      if(!Object.hasOwnProperty.call(webpackExports.c, ite)) return
      let ele = webpackExports.c[ite].exports
      if(!ele) continue
      if(filter(ele)) modules.push(ele)
    }
  }
  if (first) return modules[0]
  return modules
}
```

## Get Authorization Header

```js
XMLHttpRequest.prototype.wrappedSetRequestHeader = XMLHttpRequest.prototype.setRequestHeader; 

XMLHttpRequest.prototype.setRequestHeader = function(header, value) {
    this.wrappedSetRequestHeader(header, value);
    if(header == 'Authorization') 
        console.log('Here is your auth code:', value);
}
```

## Get Your Session Id

```js
(webpackChunkdiscord_app.push([[''],{},e=>{m=[];for(let c in e.c)m.push(e.c[c])}]),m).find(m => m?.exports?.default?.getSessionId).exports.default.getSessionId()
```

## Discord Console Self-bot by @rigwild ([Repo](https://github.com/rigwild/discord-self-bot-console))

```js
{
  var delay = ms => new Promise(res => setTimeout(res, ms))
  // prettier-ignore
  var qs = obj => Object.entries(obj).map(([k, v]) => `${k}=${v}`).join('&')

  const xSuperPropertiesObj = {
    os: 'Windows',
    browser: 'Discord Client',
    release_channel: 'stable',
    client_version: '1.0.9006',
    os_version: '10.0.22000',
    os_arch: 'x64',
    system_locale: 'en-US',
    client_build_number: 142868,
    client_event_source: null
  }

  const apiCall = (apiPath, body, method = 'GET', options = {}) => {
    if (!authHeader) throw new Error("The authorization token is missing. Did you forget to set it? `authHeader = 'your_token'`")
    const fetchOptions = {
      body: body ? body : undefined,
      method,
      headers: {
        Accept: '*/*',
        'Accept-Language': 'en-US',
        Authorization: authHeader,
        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) discord/1.0.9006 Chrome/91.0.4472.164 Electron/13.6.6 Safari/537.36',
        'X-Super-Properties': btoa(JSON.stringify(xSuperPropertiesObj))
      },
      ...options
    }
    const isFormData = body?.constructor?.name === 'FormData'
    if (!isFormData) {
      fetchOptions.headers['Content-Type'] = 'application/json'
      fetchOptions.body = JSON.stringify(body)
    }
    return fetch(`https://discord.com/api/v9${apiPath}`, fetchOptions)
      .then(res => res.json().catch(() => {}))
      .catch(console.error)
  }

  var api = {
    getMessages: (channelOrThreadId, limit = 100, params = {}) => apiCall(`/channels/${channelOrThreadId}/messages?limit=${limit ?? 100}&${qs(params)}`),
    sendMessage: (channelOrThreadId, message, tts, body = {}) => apiCall(`/channels/${channelOrThreadId}/messages`, { content: message, tts: !!tts, ...body }, 'POST'),
    replyToMessage: (channelOrThreadId, repliedMessageId, message, tts, body = {}) =>
      apiCall(`/channels/${channelOrThreadId}/messages`, { content: message, message_reference: { message_id: repliedMessageId }, tts: !!tts, ...body }, 'POST'),
    editMessage: (channelOrThreadId, messageId, newMessage, body = {}) => apiCall(`/channels/${channelOrThreadId}/messages/${messageId}`, { content: newMessage, ...body }, 'PATCH'),
    deleteMessage: (channelOrThreadId, messageId) => apiCall(`/channels/${channelOrThreadId}/messages/${messageId}`, null, 'DELETE'),

    createThread: (channelId, toOpenThreadInmessageId, name, autoArchiveDuration = 1440, body = {}) =>
      apiCall(`/channels/${channelId}/messages/${toOpenThreadInmessageId}/threads`, { name, auto_archive_duration: autoArchiveDuration, location: 'Message', type: 11, ...body }, 'POST'),
    createThreadWithoutMessage: (channelId, name, autoArchiveDuration = 1440, body = {}) =>
      apiCall(`/channels/${channelId}/threads`, { name, auto_archive_duration: autoArchiveDuration, location: 'Message', type: 11, ...body }, 'POST'),
    deleteThread: threadId => apiCall(`/channels/${threadId}`, null, 'DELETE'),

    // Use this generator: https://discord.club/dashboard
    // Click `+` at the bottom in the embed section then copy the `embed` key in the JSON output.
    // Does not work with user account anymore!
    sendEmbed: (channelOrThreadId, embed = { title: 'Title', description: 'Description' }) => apiCall(`/channels/${channelOrThreadId}/messages`, { embed }, 'POST'),

    getRoles: guildId => apiCall(`/guilds/${guildId}/roles`),
    createRole: (guildId, name) => apiCall(`/guilds/${guildId}/roles`, { name }, 'POST'),
    deleteRole: (guildId, roleId) => apiCall(`/guilds/${guildId}/roles/${roleId}`, null, 'DELETE'),

    getBans: guildId => apiCall(`/guilds/${guildId}/bans`),
    banUser: (guildId, userId, reason) => apiCall(`/guilds/${guildId}/bans/${userId}`, { delete_message_days: '7', reason }, 'PUT'),
    unbanUser: (guildId, userId) => apiCall(`/guilds/${guildId}/bans/${userId}`, null, 'DELETE'),
    kickUser: (guildId, userId) => apiCall(`/guilds/${guildId}/members/${userId}`, null, 'DELETE'),

    addRole: (guildId, userId, roleId) => apiCall(`/guilds/${guildId}/members/${userId}/roles/${roleId}`, null, 'PUT'),
    removeRole: (guildId, userId, roleId) => apiCall(`/guilds/${guildId}/members/${userId}/roles/${roleId}`, null, 'DELETE'),

    auditLogs: guildId => apiCall(`/guilds/${guildId}/audit-logs`),

    getChannels: guildId => apiCall(`/guilds/${guildId}/channels`),
    createChannel: (guildId, name, type) => apiCall(`/guilds/${guildId}/channels`, { name, type }, 'POST'),
    deleteChannel: channelId => apiCall(`/channels/${channelId}`, null, 'DELETE'),
    getChannel: channelOrThreadId => apiCall(`/channels/${channelOrThreadId}`),

    pinnedMessages: channelId => apiCall(`/channels/${channelId}/pins`),
    addPin: (channelId, messageId) => apiCall(`/channels/${channelId}/pins/${messageId}`, null, 'PUT'),
    deletePin: (channelId, messageId) => apiCall(`/channels/${channelId}/pins/${messageId}`, null, 'DELETE'),

    listEmojis: guildId => apiCall(`/guilds/${guildId}/emojis`),
    getEmoji: (guildId, emojiId) => apiCall(`/guilds/${guildId}/emojis/${emojiId}`),
    createEmoji: (guildId, name, image, roles) => apiCall(`/guilds/${guildId}`, { name, image, roles }, 'POST'),
    editEmoji: (guildId, emojiId, name, roles) => apiCall(`/guilds/${guildId}/${emojiId}`, { name, roles }, 'PATCH'),
    deleteEmoji: (guildId, emojiId) => apiCall(`/guilds/${guildId}/${emojiId}`, null, 'DELETE'),

    searchSlashCommand: (channelOrThreadId, search) => apiCall(`/channels/${channelOrThreadId}/application-commands/search?type=1&query=${search}&limit=25&include_applications=true`),
    sendSlashCommand: (guildId, channelOrThreadId, command, commandOptions = []) => {
      const formData = new FormData()
      formData.append(
        'payload_json',
        JSON.stringify({
          type: 2,
          application_id: command.application_id,
          guild_id: guildId,
          channel_id: channelOrThreadId,
          session_id: 'requiredButUnchecked',
          nonce: Math.floor(Math.random() * 1000000) + '',
          data: {
            ...command,
            options: commandOptions,
            application_command: {
              ...command
            }
          }
        })
      )
      return apiCall('/interactions', formData, 'POST')
    },

    changeNick: (guildId, nick) => apiCall(`/guilds/${guildId}/members/@me/nick`, { nick }, 'PATCH'),
    leaveServer: guildId => apiCall(`/users/@me/guilds/${guildId}`, null, 'DELETE'),

    getDMs: () => apiCall(`/users/@me/channels`),
    getUser: userId => apiCall(`/users/${userId}`),

    getCurrentUser: () => apiCall('/users/@me'),
    editCurrentUser: (username, bio, body = {}) => apiCall('/users/@me', { username: username ?? undefined, bio: bio ?? undefined, ...body }, 'PATCH'),
    listCurrentUserGuilds: () => apiCall('/users/@me/guilds'),

    setCustomStatus: (emojiId, emojiName, expiresAt, text) =>
      apiCall(`/users/@me/settings`, { custom_status: { emoji_id: emojiId, emoji_name: emojiName, expires_at: expiresAt, text: text } }, 'PATCH'),
    deleteCustomStatus: () => apiCall(`/users/@me/settings`, { custom_status: { expires_at: new Date().toJSON() } }, 'PATCH'),

    listReactions: (channelOrThreadId, messageId, emojiUrl) => apiCall(`/channels/${channelOrThreadId}/messages/${messageId}/reactions/${emojiUrl}/@me`),
    addReaction: (channelOrThreadId, messageId, emojiUrl) => apiCall(`/channels/${channelOrThreadId}/messages/${messageId}/reactions/${emojiUrl}/@me`, null, 'PUT'),
    deleteReaction: (channelOrThreadId, messageId, emojiUrl) => apiCall(`/channels/${channelOrThreadId}/messages/${messageId}/reactions/${emojiUrl}/@me`, null, 'DELETE'),

    typing: channelOrThreadId => apiCall(`/channels/${channelOrThreadId}/typing`, null, 'POST'),

    delay,
    apiCall
  }

  console.log('\n\n\n\nSelfbot loaded! Use it like this: `await api.someFunction()`')
  console.log('Abusing this could get you banned from Discord, use at your own risk!')
  console.log()
  console.log(
    'This script does **not** work with bot accounts! ' +
      'If you have a bot account, use Node.js (or a proper lib like discord.js!) with the modified script ' +
      'https://github.com/rigwild/discord-self-bot-console/discussions/4#discussioncomment-1438231'
  )
  console.log()
  console.log('Use the `id()` function to update the variable `gid` guild id and `cid` channel id to what you are currently watching.')
  console.log('https://github.com/rigwild/discord-self-bot-console')

  var gid = '' // Current guild id
  var cid = '' // Current channel id

  // Call this to update `cid` and `gid` to current channel and guild id
  var id = (log = true) => {
    gid = window.location.href.split('/').slice(4)[0]
    cid = window.location.href.split('/').slice(4)[1]
    if (log) {
      console.log(`\`gid\` was set to the guild id you are currently looking at (${gid})`)
      console.log(`\`cid\` was set to the channel id you are currently looking at (${cid})`)
    }
  }
  id(false)

  // Do not replace configuration when reusing script in same context
  if (!authHeader) {
    //
    // Set your authorization token here (or use the auto update, send a message in any chat!)
    //
    var authHeader = ''
    var autoUpdateToken = true
  }

  if (!XMLHttpRequest_setRequestHeader) {
    var XMLHttpRequest_setRequestHeader = XMLHttpRequest.prototype.setRequestHeader
  }
  // Auto update the authHeader when a request with the token is intercepted
  XMLHttpRequest.prototype.setRequestHeader = function () {
    if (autoUpdateToken && arguments[0] === 'Authorization' && authHeader !== arguments[1]) {
      authHeader = arguments[1]
      console.log(`Updated the Auth token! <${authHeader.slice(0, 50)}...>`)
    }
    XMLHttpRequest_setRequestHeader.apply(this, arguments)
  }
}
```

# Not Discord-Specific, but still useful

## Design Mode

```js
document.designMode = 'on'
```

## Change Discord Title

```js
var title = 'Your Title'

document.getElementsByClassName("wordmarkWindows-2dq6rw wordmark-2u86JB")[0].innerHTML = `<span style='font-size:15px'>${title}</span>`
```

![image](https://user-images.githubusercontent.com/91196395/200526504-1b7fefff-1d5f-4d31-b2af-fe5ab0089cf2.png)

### Please tell me if something is broken, outdated, or if I need to add something!

# Behind the Scenes and Discord Framework

## Discord CDN Syntax

### Banner CDN Link

<table>
  <tr><th></th><th>Example</th></tr>
  <tr><td>Base Banner CDN Link</td><td>https://cdn.discordapp.com/banners/</td></tr>
  <tr><td>User Id</td><td>904043694334824498</td></tr>
  <tr><td>Slash</td><td>/</td></tr>
  <tr><td>Banner Hash</td><td>d0015e2f9ac73291edf7a7b33b38c738</td></tr>
  <tr><td>File Format</td><td>.png</td></tr>
  <tr><td>Question Mark</td><td>?</td></tr>
<tr><td>Size Parameter</td><td>size=300</td></tr>
</table>

## Discord Token Syntax

<table>
  <tr><th></th><th>Example</th></tr>
  <tr><td>User ID Encoded in Base64</td><td>NTzQvPcLBacBmgajXQc7QAaU</td></tr>
  <tr><td>Dot</td><td>.</td></tr>
  <tr><td>Timestamp -epoch(1293840000) converted to base64</td><td>XCgboz</td></tr>
  <tr><td>Dot</td><td>.</td></tr>
  <tr><td>HMAC consiting of 27 chars (uppercase/lowercase letters, numbers, - or _)</td><td>c4t51kFWSEmdmaPnKoyUuu8E78E</td></tr>
</table>
<br>
Diagram Version: <br>
<img src="https://user-images.githubusercontent.com/34555296/120932740-4ca47480-c6f7-11eb-9270-6fb3fbbd856c.png"></img>

## Discord Id Syntax

<table>
    <thead>
        <tr>
            <th scope="col">Field</th>
            <th scope="col">Bits</th>
            <th scope="col">Number of bits</th>
            <th scope="col">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Timestamp</td>
            <td>63 to 22</td>
            <td>42 bits</td>
            <td>Milliseconds since Discord Epoch, the first second of 2015 or 1420070400000.</td>
        </tr>
        <tr>
            <td>Internal worker ID</td>
            <td>21 to 17</td>
            <td>5 bits</td>
            <td></td>
        </tr>
        <tr>
            <td>Internal process ID</td>
            <td>16 to 12</td>
            <td>5 bits</td>
            <td></td>
        </tr>
        <tr>
            <td>Increment</td>
            <td>11 to 0</td>
            <td>12 bits</td>
            <td>For every ID that is generated on that process, this number is incremented</td>
        </tr>
    </tbody>
</table>

### How To Convert Discord ID > Date

<img src="https://i.imgur.com/wAkzCtk.png"></img> <br><br>

**In Javascript:** `new Date((id / 4194304) + 1420070400000);` <br>
```js
function getCreationDate(id) { 
  return new Date((id / 4194304) + 1420070400000); 
}
getCreationDate("insertId")

const getTime = (id) => {
  return ((Number(BigInt.asUintN(64, id) >> 22n)) + 1420070400000) / 1000 | 0
}
getTime("instertId")
```
**Example:** `new Date((622716865428324353 / 4194304) + 1420070400000);` <br>
![image](https://user-images.githubusercontent.com/67203548/127029200-840e81dc-532d-4b74-959e-05c4395cc5ef.png)

## Discord User Flags

| Flag    | Bitwise | Internal Name              | Description                                       | Public |
|---------|---------|----------------------------|---------------------------------------------------|--------|
| 1       | 1<<0    | STAFF                      | Discord Employee                                  | ✓      |
| 2       | 1<<1    | PARTNER                    | Discord Partner                                   | ✓      |
| 4       | 1<<2    | HYPESQUAD                  | HypeSquad Events                                  | ✓      |
| 8       | 1<<3    | BUG_HUNTER_LEVEL_1         | Bug Hunter Level 1                                | ✓      |
| 16      | 1<<4    | MFA_SMS                    | SMS recovery for 2FA enabled                      |        |
| 32      | 1<<5    | PREMIUM_PROMO_DISMISSED    | Dismissed Nitro promotion                         |        |
| 64      | 1<<6    | HYPESQUAD_ONLINE_HOUSE_1   | HypeSquad Online House Bravery                    | ✓      |
| 128     | 1<<7    | HYPESQUAD_ONLINE_HOUSE_2   | HypeSquad Online House Brilliance                 | ✓      |
| 256     | 1<<8    | HYPESQUAD_ONLINE_HOUSE_3   | HypeSquad Online House Balance                    | ✓      |
| 512     | 1<<9    | PREMIUM_EARLY_SUPPORTER    | Early Supporter                                   | ✓      |
| 1024    | 1<<10   | TEAM_USER                  | Team User                                         | ✓      |
| 2048    | 1<<11   | INTERNAL_APPLICATION       | An internal flag accidentally leaked to the client's private flags. Relates to partner/verification applications but nothing else is known     |        |
| 4096    | 1<<12   | SYSTEM                     | System User                                       | ✓      |
| 8192    | 1<<13   | HAS_UNREAD_URGENT_MESSAGES | Has an unread system message                      |        |
| 16384   | 1<<14   | BUG_HUNTER_LEVEL_2         | Bug Hunter Level 2                                | ✓      |
| 32768   | 1<<15   | UNDERAGE_DELETED           | Pending deletion for being underage in DOB prompt |        |
| 65536   | 1<<16   | VERIFIED_BOT               | Verified Bot                                      | ✓      |
| 131072  | 1<<17   | VERIFIED_DEVELOPER         | Early Verified Bot Developer                      | ✓      |
| 262144  | 1<<18   | CERTIFIED_MODERATOR        | Discord Certified Moderator                       | ✓      |
| 524288  | 1<<19   | BOT_HTTP_INTERACTIONS      | Bot has set an interactions endpoint url          | ✓      |
| 1048576 | 1<<20   | SPAMMER                    | User is disabled for being a spammer              | ✓      |
| 2097152 | 1<<21   | DISABLE_PREMIUM            | Disables Nitro Features                           |        |
| 8589934592 | 1<<33 | HIGH_GLOBAL_RATE_LIMIT  | Account has a high global ratelimit                  |        |
| 	17179869184 | 1<<34   | DELETED               | Account has been deleted                          |        |
| 34359738368 | 1<<35 | DISABLED_SUSPICIOUS_ACTIVITY | Account has been disabled for suspicious activity                      |        |
| 68719476736 | 1<<36   | SELF_DELETED            | Account was deleted by the user                           |        |
| 137438953472 | 1<<37   | PREMIUM_DISCRIMINATOR            | User has a premium discriminator                           |        |
| 274877906944 | 1<<38   | USED_DESKTOP_CLIENT            | User has used the desktop client                           |        |
| 549755813888 | 1<<39   | USED_WEB_CLIENT            | User has used the web client                           |        |
| 1099511627776 | 1<<40   | USED_MOBILE_CLIENT            | User has used the mobile client                           |        |
| 2199023255552 | 1<<41   | DISABLED            | User is currently temporarily or permanently disabled                       |        |
| 8796093022208 | 1<<43   | VERIFIED_EMAIL            | User has a verified email                           |        |
| 17592186044416 | 1<<44   | QUARANTINED            | User account is quarantined                           |        |

## Discord Application Flags

<html>
<body>
<!--StartFragment-->

Name | Number | Description
-- | -- | --
EMBEDDED_RELEASED | 2 (1 << 1) | Indicates if an embedded app is available to play
MANAGED_EMOJI | 4 (1 << 2) | Indicates if the app has the ability to create Twitch-style emojis
GROUP_DM_CREATE | 16 (1 << 4) | Indicates if the app has permission to create group DMs
RPC_PRIVATE_BETA | 32 (1 << 5) | Allows the application to access the local RPC server
ALLOW_ASSETS | 256 (1 << 8) | Allows the application to create activity assets
ALLOW_ACTIVITY_ACTION_SPECTATE | 512 (1 << 9) | Allows the application to enable activity spectating
ALLOW_ACTIVITY_ACTION_JOIN_REQUEST | 1024 (1 << 10) | Allows the application to enable join requests for activities
RPC_HAS_CONNECTED | 2048 (1 << 11) | Indicates whether the application has accessed the local RPC server before
GATEWAY_PRESENCE | 4096 (1 << 12) | Intent required for bots in 100 or more servers to receive presence_update events
GATEWAY_PRESENCE_LIMITED | 8192 (1 << 13) | Intent required for bots in under 100 servers to receive presence_update events
GATEWAY_GUILD_MEMBERS | 16384 (1 << 14) | Intent required for bots in 100 or more servers to receive member-related events like guild_member_add
GATEWAY_GUILD_MEMBERS_LIMITED | 32768 (1 << 15) | Intent required for bots in under 100 servers to receive member-related events like guild_member_add
VERIFICATION_PENDING_GUILD_LIMIT | 65536 (1 << 16) | Indicates unusual growth of an app that prevents verification
EMBEDDED | 131072 (1 << 17) | Indicates if an app is embedded within the Discord client
GATEWAY_MESSAGE_CONTENT | 262144 (1 << 18) | Intent required for bots in 100 or more servers to receive message content
GATEWAY_MESSAGE_CONTENT_LIMITED | 524288 (1 << 19) | Intent required for bots in under 100 servers to receive message content
EMBEDDED_FIRST_PARTY | 1048576 (1 << 20) | Indicates a first-party embedded app
APPLICATION_COMMAND_BADGE | 8388608 (1 << 23) | Indicates if an app has registered global application commands

<!--EndFragment-->
</body>
</html>

## Discord Activities

### MAX CONCURRENT ACTIVITIES
| Guild Tier | Max concurrent activities |
| --- | --- |
|  Tier 0 | 2 |
|  Tier 1 | 3 |
|  Tier 2 | 5 |
|  Tier 3 | Number.MAX_SAFE_INTEGER = 9007199254740991 |

### Stable versions
| Icon | Application ID | Application name | Boost level | Max participants |
| --- | --- | --- |:---:|:---:|
| ![Icon](https://cdn.discordapp.com/app-icons/755600276941176913/4e0fd3bf009282c0ecd1fb010e621f28.webp?size=80) | 755600276941176913 | YouTube Together (Deprecated. Replaced by 'Watch Together') | 0 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/880218394199220334/ec48acbad4c32efab4275cb9f3ca3a58.webp?size=80) | 880218394199220334 | Watch Together | 0 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/755827207812677713/e594da3ca4520c7edde5b59948e97cdc.webp?size=80) | 755827207812677713 | Poker Night | 1 | 7 |
| ![Icon](https://cdn.discordapp.com/app-icons/773336526917861400/0227b2e89ea08d666c43003fbadbc72a.webp?size=80) | 773336526917861400 | Betrayal.io | 0 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/814288819477020702/0cafdebe76abfd7d8d9b015c2060512e.webp?size=80) | 814288819477020702 | Fishington.io | 0 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/832012774040141894/3b3981ddf67c8702920fae10b5f123ed.webp?size=80) | 832012774040141894 | Chess In The Park | 1 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/902271654783242291/0fbc3e38ea4b26c47d8001eff6b94a7b.webp?size=80) | 902271654783242291 | Sketch Heads | 0 | 16 |
| ![Icon](https://cdn.discordapp.com/app-icons/879863686565621790/0096355142a9b00bc2676ec09b9c8dbc.webp?size=80) | 879863686565621790 | Letter League (Formerly known as 'Letter Tile') | 1 | 8 |
| ![Icon](https://cdn.discordapp.com/app-icons/879863976006127627/930f9cfe504211a130419e731babc597.webp?size=80) | 879863976006127627 | Word Snacks | 0 | 8 |
| ![Icon](https://cdn.discordapp.com/app-icons/852509694341283871/9a4a52c760994654a416740ae0b19fbb.webp?size=80) | 852509694341283871 | SpellCast | 1 | 100 |
| ![Icon](https://cdn.discordapp.com/app-icons/832013003968348200/97e50fed67f44802dbb4901d74a6f9a1.webp?size=80) | 832013003968348200 | Checkers In The Park (Formerly known as 'CG3 Prod'.) | 1 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/832025144389533716/6fe6e3dda7657b83758693205a833aa1.webp?size=80) | 832025144389533716 | Blazing 8s (Formerly known as 'Ocho' & 'CG4 Prod')| 1 | 8 |
| ![Icon](https://cdn.discordapp.com/app-icons/945737671223947305/12ee915c2f75d7f2c7d551819534f158.webp?size=80) | 945737671223947305 | Putt Party | 1 | 8 |
| ![Icon](https://cdn.discordapp.com/app-icons/903769130790969345/c4d8b95b8f06b1ff8cf2b769e94505a8.webp?size=80) | 903769130790969345 | Land.io | 1 | 16 |
| ![Icon](https://cdn.discordapp.com/app-icons/947957217959759964/b485f75e95e6486a758a4aa5db3352f4.webp?size=80) | 947957217959759964 | Bobble League | 1 | 8 |
| ![Icon](https://cdn.discordapp.com/app-icons/976052223358406656/4f86c19a69cc3002d1b52f7a22687adf.webp?size=80) | 976052223358406656 | Ask Away | 0 | 10 |
| ![Icon](https://cdn.discordapp.com/app-icons/950505761862189096/6f547114b2979b8bc83e4ba91b4d770d.webp?size=80) | 950505761862189096 | Know What I Meme | 0 | 8 |
| ![Icon](https://cdn.discordapp.com/app-icons/1006584476094177371/eace9c231b505f0c96fba27d1795c31a.webp?size=80) | 1006584476094177371 | Bash Out | 1 | 16 |

### Development versions
| Icon | Application ID | Application name | Boost level | Max participants |
| --- | --- | --- |:---:|:---:|
| ![Icon](https://cdn.discordapp.com/app-icons/763133495793942528/3bf3592c0949620f0e76cb28ab7affd9.webp?size=80) | 763133495793942528 | PN Dev | 0 | 7 |
| ![Icon](https://cdn.discordapp.com/app-icons/880218832743055411/3f135503dc803ce7bcf555c769b3f577.webp?size=80) | 880218832743055411 | Watch Together Dev | 0 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/902271746701414431/e3681f5161229ff041e9642e93e6a241.webp?size=80) | 902271746701414431 | Sketch Heads Dev | 0 | 16 |
| ![Icon](https://cdn.discordapp.com/app-icons/879863753519292467/09a8b98f5f5c219e7befa6693c7f73e4.webp?size=80) | 879863753519292467 | Letter League Dev (Formerly known as 'Letter Tile Dev') | 0 | 8 |
| ![Icon](https://cdn.discordapp.com/app-icons/879864010126786570/1e47e5a033aa7a853fdea22534292bfe.webp?size=80) | 879864010126786570 | Word Snacks Dev | 0 | 32 |
| ![Icon](https://cdn.discordapp.com/app-icons/832012586023256104/3b3981ddf67c8702920fae10b5f123ed.webp?size=80) | 832012586023256104 | CG 2 Dev | 0 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/832012682520428625/97e50fed67f44802dbb4901d74a6f9a1.webp?size=80) | 832012682520428625 | CG 3 Dev (Also known as checkers in the park) | 0 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/832013108234289153/94ccfd4c1c0749b1ccf7a52feefb0468.webp?size=80) | 832013108234289153 | CG4 Dev | 0 | 8 |
| ![Icon](https://cdn.discordapp.com/app-icons/910224161476083792/e69a66ab92d97173757b87ede8b02c36.webp?size=80) | 910224161476083792 | Putt Party Dev | 0 | 8 |

### Staging versions
| Icon | Application ID | Application name | Boost level | Max participants |
| --- | --- | --- |:---:|:---:|
| ![Icon](https://cdn.discordapp.com/app-icons/763116274876022855/532775a7b8fd36fadefe18e0ebc209a0.webp?size=80) | 763116274876022855 | PN Staging | 0 | 7 |
| ![Icon](https://cdn.discordapp.com/app-icons/832012730599735326/3b3981ddf67c8702920fae10b5f123ed.webp?size=80) | 832012730599735326 | CG2 Staging | 0 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/832012938398400562/97e50fed67f44802dbb4901d74a6f9a1.webp?size=80) | 832012938398400562 | CG3 Staging | 0 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/832025061657280566/832ff736821811d7f41d0ff09b374ccb.webp?size=80) | 832025061657280566 | CG4 Staging | 0 | 8 |
| ![Icon](https://cdn.discordapp.com/app-icons/893449443918086174/74d41d680b96eec08562164988be671a.webp?size=80) | 893449443918086174 | SpellCast Staging | 0 | 100 |
| ![Icon](https://cdn.discordapp.com/app-icons/945732077960188005/27881d08b84784b2c98a5aae921c09ae.webp?size=80) | 945732077960188005 | Putt Party Stg | 0 | null |

### QA versions
| Icon | Application ID | Application name | Boost level | Max participants |
| --- | --- | --- |:---:|:---:|
| ![Icon](https://cdn.discordapp.com/app-icons/801133024841957428/b09940bb01c6f0aa2ea4288d5e08218f.webp?size=80) | 801133024841957428 | Poker QA | 0 | 7 |
| ![Icon](https://cdn.discordapp.com/app-icons/832012815819604009/3b3981ddf67c8702920fae10b5f123ed.webp?size=80) | 832012815819604009 | CG2 QA | 0 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/832012894068801636/97e50fed67f44802dbb4901d74a6f9a1.webp?size=80) | 832012894068801636 | CG 3 QA | 0 | Unlimited |
| ![Icon](https://cdn.discordapp.com/app-icons/832025114077298718/ee2edef3edb605a83e5331de070fd49c.webp?size=80) | 832025114077298718 | CG4 QA | 0 | 8 |
| ![Icon](https://cdn.discordapp.com/app-icons/945748195256979606/5f8a388110138fb6fa586eedc73e075a.webp?size=80) | 945748195256979606 | Putt Party QA | 0 | 8 |

### Unknown applications
| Icon | Application ID | Application name | Boost level | Max participants |
| --- | --- | --- |:---:|:---:|
| ![Icon](https://cdn.discordapp.com/app-icons/880559245471408169/44c30f5fb9ec99753984f50c47524fc9.webp?size=80)| 880559245471408169 | iframe-playground | 0 | 100 |
|   | 832025993019260929 | CGSample | 0 | 100 |

### Deleted applications
| Application ID | Application name |
| --- | --- |
| ![Icon](https://cdn.discordapp.com/app-icons/879863881349087252/7bb9cd8518723b74c9a1d260cd177f24.webp?size=80) | 879863881349087252 | Awkword | 0 | 12 |
| ![Icon](https://cdn.discordapp.com/app-icons/879863923543785532/dfd06404877f7bb863430d32c43480fd.webp?size=80) | 879863923543785532 | Awkword Dev | 0 | 32 |
| ![Icon](https://cdn.discordapp.com/app-icons/878067389634314250/9bd4b9e21576f14f09a9284d45640a9e.webp?size=80) | 878067389634314250 | Doodle Crew (Deprecated. Replaced by 'Sketch Heads') | 0 | 16 |
| ![Icon](https://cdn.discordapp.com/app-icons/878067427668275241/50be5b98e871a395aa160fefdba5b596.webp?size=80) | 878067427668275241 | Doodle Crew Dev (Deprecated. Replaced by 'Sketch Heads Dev') | 0 | 16 |
| ![Icon](https://cdn.discordapp.com/app-icons/879864070101172255/0214576f3c33e4026a72f248c11d2292.webp?size=80) | 879864070101172255 | Sketchy Artist | 0 | 12 |
| ![Icon](https://cdn.discordapp.com/app-icons/879864104980979792/86df8c0d2ab678bba9ac560d42a6f9aa.webp?size=80) | 879864104980979792 | Sketchy Artist Dev | 0 | 12 |
| ![Icon](https://cdn.discordapp.com/app-icons/891001866073296967/ab9c4e0add01dc8934a336bbc947738e.webp?size=80) | 891001866073296967 | Decoders Dev | 0 | 32 |
| 1006986333539029022 | Clone - Watch Together | 0 | null |
| 832012854282158180 | Delete Me Calla (Formerly known as 'putt dis' 'click dis' and 'Putts'.) |
| 832025179659960360 | Discord Game 14 |
| 832025219526033439 | Discord Game 15 |
| 832025249335738428 | Discord Game 16 |
| 832025333930524692 | Discord Game 17 |
| 832025385159622656 | Discord Game 18 |
| 832025431280320532 | Discord Game 19 |
| 832025470685937707 | Discord Game 20 |
| 832025799590281238 | Discord Game 21 |
| 832025857525678142 | Discord Game 22 |
| 832025886030168105 | Discord Game 23 |
| 832025928938946590 | Discord Game 24 |

## Discords Brand / Bot Ids

Discord System message account ID: - 643945264868098049

Discord Community updates account ID - 669627189624307712

Discord Owner Account ID - 21414249976823808

Clyde Bots ID - 1

Note: Some of them you cant mention because of how IDs work

## Discords Internal Server Structure
Check out this article about Reverse Engineering Discord, and the proof that Discord decrypts your encrypted data: <a href="https://medium.com/tenable-techblog/lets-reverse-engineer-discord-1976773f4626">https://medium.com/tenable-techblog/lets-reverse-engineer-discord-1976773f4626</a><br>
They can also read your messages (e.g. in DM's), log all edits and deleted messages and record your voice calls.

<b>Would just like to state myself that there has been multiple periods where discord hasn't been able to find edited or deleted messages</b>
<br>
![grafik](https://user-images.githubusercontent.com/55095883/116671170-e9f5e580-a9a0-11eb-98f9-3bcd65b9fdbf.png)

How sending Audio/Video Messages in Discord Works.

### Domains

| Domain                | Description                              |
|-----------------------|------------------------------------------|
| dis.gd                | Marketing URL shortener                  |
| i.dis.gd              | Internal URL shortener                   |
| discord.co            | Admin panel, internal tools              |
| discord.com           | New app, marketing website, API host     |
| discord.design        | Dribbble profile shortlink               |
| discord.dev           | Developer site shortlinks                |
| discord.gg            | Invite shortlinks, Gateway host          |
| discord.gift          | Gift shortlinks                          |
| discord.gifts         | Another gift shortlinks domain           |
| discord.media         | Voice servers                            |
| discord.new           | Template shortlinks                      |
| discord.store         | Merch store                              |
| discord.tools         | Internal tools                           |
| discordapp.com        | Old app, marketing website, and API; CDN |
| discordapp.net        | Media Proxy, Client Downloads            |
| discordmerch.com      | Merch store                              |
| discordpartygames.com | Voice channel activity API host          |
| discord-activities.com| Voice channel activity API host          |
| discordactivities.com | Voice channel activity data management   |
| discordsays.com       | Voice channel activity host              |
| discordstatus.com     | Status page                              |

### Other Domains

| Domain                    | Description                                                         |
|---------------------------|---------------------------------------------------------------------|
| airhorn.solutions         | [API implementation example](https://github.com/discord/airhornbot) |
| airhornbot.com            | ^                                                                   |
| bigbeans.solutions        | [April Fools 2017](https://youtu.be/9Z4GW6Vd6NI)                    |
| watchanimeattheoffice.com | HypeSquad form placeholder/meme                                     |

### Unused Domains

| Domain         |
|----------------|
| discordapp.io  |
| discordcdn.com |


## Discord Webpack Modules

<a href='https://rauenzi.github.io/BDPluginLibrary/docs/modules_discordmodules.js.html'>List of Modules that are used in a bdApi plugin that requires Zere's Plugin Library</a>

## Running scripts on load/reload
If you want to automate scripts being run on load/reload head over to 
```dir
%localappdata%\Discord\app-{version}\modules\discord_dispatch-1\discord_dispatch
```
and make a new file named 
```dir
scripts.js
```
and insert your scripts that you want to load on discord startup/reload into that file, then add this line to the **index.js** file inside of the folder:
```js
require('./scripts.js')
```
and then finally start up Discord and enjoy!

-----------------------

<td><table cellspacing="0" cellpadding="0" border="0"><tr><td style="font-family: Roboto, sans-serif; font-weight: 700; font-size: 16px; line-height: 19px; color: rgb(0, 40, 72); padding: 0px 0px 4px;">Raz</td></tr><tr><td style="font-family: Roboto, sans-serif; font-weight: 700; font-size: 10px; line-height: 12px; color: rgb(174, 192, 209); padding: 0px 0px 4px; text-transform: uppercase;">Experienced Programmer</td></tr><!----><tr><td style="padding: 0px; font-size: 10px; line-height: 12px;"><a href="https://github.com/Raz-js" style="font-family: Roboto, sans-serif; font-weight: 700; color: rgb(67, 147, 207); text-decoration: none;">Document Revised By Raz</a></td></tr></table></td></tr></table>

### GH Pages Styling Below! Ignore Below!

<style>body, html { background:black;color:limegreen; } .markdown-body img { background-color:darkslategrey;border-radius:23px; }</style>
