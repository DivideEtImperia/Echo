# Need help?
You can visit our server and ask any questions: https://discord.gg/0pTKzt2BDInBOrxL <Br>
**__ISSUES:__** Make sure to give Echo the full permissions he asks for.  
We're working on any role issues we're still having. However **Most should be fixed!**  
<Br>
<br>
## Want to donate?
We could always use any support to help keep our server up.  
right now we're running a small server. so all help is appreciated! <a href="https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=proxikal2%40gmail%2ecom&lc=US&item_name=Echo%20Bot&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted" target="_new">Donate to Echo Today!</a>  
  
## Index
[Word Filter Examples](https://github.com/proxikal/Echo/blob/master/README.md#some-other-examples)  
[Meme and Joke Command](https://github.com/proxikal/Echo/blob/master/README.md#build-the---meme-or---jokes-command)  
[Cats Command](https://github.com/proxikal/Echo/blob/master/README.md#build-the---cats-command-in-your-server)  
[Giphy Command](https://github.com/proxikal/Echo/blob/master/README.md#build-the---giphy-command-in-your-server)  
[Giveme Command](https://github.com/proxikal/Echo/blob/master/README.md#build-the---giveme-command-in-your-server)  
[NSFW Commands](https://github.com/proxikal/Echo/blob/master/README.md#build-the-nsfw-commands)  
[Kick\Ban Warning](https://github.com/proxikal/Echo/blob/master/README.md#set-warning-for-kickban)  
[Emoji Guide](https://github.com/proxikal/Echo/blob/master/README.md#emojis-guide)  
  
  
  
### Echo's commands
<pre>
--addmaster, --delmaster, --autorole, --bye, --getid, --rolecolor
--greet, --prefix, --ban, --kick, --give, --giveme
--take, --giphy, --auto, --delauto --viewauto, --wipeauto
--mute, --unmute, --locateip, --cats, --allowlinks, --denylinks
--setpunish, --channelid, --botrole
--mkchan, --invites, --mkinvite, --nsfw, --grabars --putars
--upskirt, --lesbians, --celebs, --twinks, --fatgirls
--space, --sky, --cars, --trucks
</pre>
  
### Admin\Staff Emojis
```php
:ripakiara: :ripdoorstop: :ripedible:
:ripproxy: :ripkenson:
```
   
### League of Legends Emojis
```php
:score: :told you: :baby please: :yummy:
:gotcha: :no more: :hell yeah: :deal with it:
:love you: :ffs: :haha: :too hot:
:why: :sleep zzz: :oh my god:
:ouch: :cmon guys: :sleepy time:
:yeah ok: :hey ladies: :vengeance:
:happy birthday: :seriously: :peekaboo:
:omfg: :solotop: :jungle: :toplane:
:save a life:
More coming soon.
```
  
### Twitch Emojis
```php
:seemsgood: :biblethump: :kappa: :frankerz:
:elegigiggle: :minglee: :feelsgoodman: :feelsbadman:
:pogchamp: :swiftrage: :rip: :gaben: :wutface:
```
check out [The Emoji Guide](https://github.com/proxikal/Echo/blob/master/README.md#emojis-guide) For the full list (In Progress)  
Will be updating the readme to better explain how to use!  
  
### Submit your own emoji!
Join our server [Click Here!](https://discord.gg/0pTKzt2BDInBOrxL) Private Message Proxy  
the emoji has to be `transparent` `.png` extension only. and `100x100` pixels in size.  
These images will be seen by everyone. So no NSFW content, nothing vulgar.  
Pm me the name you want. No ascii characters.  
acceptable names: `:yournamehere:` or `:your name here:`, `:your-name-here:`, `:your_name_here:`  
**__HINT:__** make sure discord doesn't have an emoji with your name. or i'll shift the naming.  
  
  
<pre>
rolecolor- Example: --rolecolor #FF0000 Role Name
bye - Example: --bye {user} has left the server
autorole - Example: --autorole Role Name auto assigns role to new members.
autorole - (<b>Silent:</b>) --autorole -s Role Name auto assigns a role to a new member silently.
botrole - Example: --botrole Role Name auto assigns a role to new bot accounts that join your server.
botrole - (<b>Silent:</b>) --botrole -s Role Name auto assigns roles to new bots silently.
greet - Example: --greet Welcome {user} if you need any help ask Proxy! you can use {/user} for non-mentions.
give - Gives user a role. Example: --give @user Role Name
take - Takes a role away from someone. Example: --take @user Role Name
auto - --auto trigger=response{keys}{keys} or: --auto &trigger=response{keys}{keys}
allowauto - true or false (true: bot commanders can add\edit your A.R.S)
delauto - deletes your auto response. if you added {params} you need to add it in the --delauto as well.
viewauto - views a list of your auto responses
wipeauto - deletes your A.R.S File.
nsfw - true or false. Allows NSFW commands like --upskirt, --lesbian etc..
grabars - Echo will send you your autoresponse.json file to edit manually.
putars - you need to link directly to your autoresponse.json file. (updates your ars file!)
</pre>

# Auto Response System Keys
> <b>You no longer need to initiate by typing</b> `--auto`  
you can just start adding keys!  
  
Ok first let's look at the trigger section.  
You want to set this to whatever word/sentence you want Echo to respond to.  
  
  
<b>NEW: You can use the {params} key in the trigger to catch their text!</b>  
`--auto &giveme {params}={role:{params}}{req:Owner}You've assumed the role {params}`  
The example above `requires` you to have the role `Owner` and will give you  
whatever role you type (*As long as the role exists*) for example: `giveme Staff`  
  
  
If you want to use regex you add the <b>&</b> key before the word Example Below:  
`--auto &word=The Response here!`  
Want to add a work like `ass` to the word filter? but don't want to catch `mass`?  
Add a space after the word. this will assure it only triggers on the word! Example Below:  
`--auto &ass =The Response here!`  
  
Ok, now let's look at the <b>Response</b> section and all the keys you can use!  
<b>Keys</b> are surrounded by obraces. `{key}` Echo will replace these keys with data!  
Here's a list:  
```php
{pm}                // Private messages the response instead of in the server.
{user}              // Mentions the users name.
{/user}             // Just says the users name (without mention)
{del}               // deletes the users message.
{kick}              // Kicks the user. (Won't kick bot commanders or the owner)
{ban}               // Bans the user. (Won't ban bot commanders or the owner)
{role:Role Name}    // Gives the user a specific role.
{exc:Role Name}     // Excludes One or more roles from a trigger. {exc:Role1,Role2,Role3}
{alert:YOURID}      // Alerts one or more people via pm. to get id: --getid @User
{chan}              // Says the current channel name.
{pref}              // Says Echo's current prefix.
{greet}             // Says your current greet message if set.
{bye}               // Says your current bye message if set.
{ismaster}          // True or False if the user is a Bot Commander.
{listroles}         // lists the users roles.
{allroles}          // lists all roles in your server.
{joined}            // shows the date and time when someone joined your server.
{channels}          // lists all channels in your server.
{meme}              // shows a random meme.
{joke}              // shows a random joke.
{params}            // catches the users text. REQUIRES: {params} key in the trigger as well!
{req:Role Name}     // Requires the user to have the role to use the trigger.
{ass}               // shows random images of asses.
{boobs}             // shows random images of boobs.
{warn:number}       // warns x amount of times before kicking\banning: only works with {ban} or {kick}
{msg:warn msg}      // only works with {warn} key: The warning message before Echo kicks\Bans.
```
  
Will add more every day!
  
### Some cool stuff!
Alright let's make a **"Server Info"** command  
the purpose is to keep you updated on what your greet\bye or prefix is.  
  
in your server type this exactly:  
```php
--auto .server=
SERVER INFO
--------------
prefix: {pref}
greet: {greet}
bye: {bye}
roles: {allroles}
channels: {channels}
--------------
```
Now when you type **.server** Echo will display your prefix, greet and bye message also the curent channel.  
  
  
Let's make a **whoami?** command  
```php
--auto &whoami=
you: {/user}
commander: {ismaster}
channel: {chan}
roles: {listroles}
```
pretty neat huh? :)  
  
### Some other examples:

Let's filter the word `fuck` and have Echo delete the msg, pm the user and than kick them.  
We're going to exclude 3 roles `Staff` `Owner` and `Bots` for this example  
```php
--auto &fuck={del}{pm}{kick}You've been kicked for swearing.{exc:Staff,Owner,Bots}
```
  
Let's have Echo PM you everytime someone uses your trigger.  
in this example we'll use @Proxy as the trigger.  
```php
--auto &<@146046383726657536>={alert:146046383726657536}I have alerted proxy that you need help.
```
You can either get your id with `--getid @User` or you can add the @Proxy first, and than add the & symbol after.  

### Build the `--meme` or `--jokes` command
```php
--auto --meme={meme}
```
  
```php
--auto --joke={joke}
```
  
### Build the `--cats` command in your server.
```php
--auto --cats={cats}
```

### Build the `--giphy` command in your server.
```php
--auto &--giphy {params}={giphy}
```
let's explain the code above a little. as you see the new `{params}` key  
you can add the `{params}` key to catch text. and than you could use the key in the response  
to make echo say their text back. **this is not required for the {giphy} key**  

### Build the `--giveme` command in your server.
```php
--auto &--giveme {params}={role:{params}}{req:Owner}You've assumed the role **{params}**
```
the above code gives you any role you type. requires you to have the role `Owner`  
example of above: `--giveme Staff` will give you the role `Staff`  

### Build the NSFW commands
```php
--auto --ass={ass}
```
  
```php
--auto --boobs={boobs}
```
  
### Set Warning for kick\ban
```php
--auto &fuck={del}{warn:2}{msg:You have been warned!}{kick}I have kicked {user} for swearing.
```
the above code will delete the user's message. Warn twice with "**You have been warned**"  
and than kick the user if their warns exceed or equal to 2.  
You can change the **{kick}** key to the **{ban}** key if you want.
  
### Emojis Guide
<img src="https://raw.githubusercontent.com/proxikal/Echo/master/emojis1.png">  
<img src="https://raw.githubusercontent.com/proxikal/Echo/master/emojis2.png">  
<img src="https://raw.githubusercontent.com/proxikal/Echo/master/emojis3.png">  
<img src="https://raw.githubusercontent.com/proxikal/Echo/master/emojis4.png">
More updated daily!
