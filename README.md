# List of Minecraft: Bedrock Edition URI protocol links
All of these links were gathered by reverse engineering the latest Windows client binary (1.21.2 at the time). **Prefix each with `minecraft://`.**

## `?showHowToPlayScreen=1`
Shows the how to play screen

## `oculus_launched <unknown>`
Seems like this one shows a toast and then sets the input state to VR

## `?addExternalServer=<server name: string>|<ip: string>:<port: number>`
Adds an external server to the server list

## `?showStoreOffer=<item: UUID>`
Shows an item on the marketplace

## `?showOfferCollection=<unknown>`
Not sure what this one does

## `?showStoreHomeScreen=1`
Shows the marketplace home screen

## `openStore <no arguments>`
Same thing as above, just simpler

**NOTE:** You can mix openStore and showStoreOffer like so: `minecraft://openStore/?showStoreOffer=<item>`. This is probably possible with other links.

## `?showMineCoinOffers=1`
Shows the modal for purchasing Minecoins

## `?openMarketplaceInventory=<tab name: Owned|RealmsPlusCurrent|RealmsPlusRemoved|Subscriptions>`
Opens the current user's Marketplace inventory

## `?openCsbPDPScreen=<tab name: Home|Content|Faq|Subscribe>`
Opens the screen for purchasing the Marketplace Pass

## `openServersTab <no arguments>`
Opens the servers tab in the play menu

## `showDressingRoomOffer?offerID=<item: UUID>`
Shows a cosmetic item in the dressing room

## `showProfileScreen <no arguments>`
Opens the dressing room

## `joinGathering?gatheringId=<unknown: string>`
Probably for in-game events (like the Mob Vote)

## `acceptRealmInvite?inviteID=<realm invite code: string>`
Accepts a Realms invite code

## `connectToRealm? (realmId=<realm id: string> OR inviteID=<realm invite code: string>)`
Connects to a Realm

## `?slashcommand=<command: string>`
Executes a command in the current world

## `fromtempfile`
Seems to be unused

## `originalpath`
This seems to do something with resource packs

## `?import=<path: string>`
Imports content, could possibly be any type

## `?importload=<arguments unknown>`
Not sure what this one does

## `?importpack=<path: string (*.mcpack)>`
Imports a resource or behavior pack

## `?importaddon=<path: string (*.mcaddon)>`
Imports an addon

## `?importtemplate=<path: string (*.mctemplate)>`
Imports a world template

## `?load=<local level id: string>`
Loads a local world

## `connect <many arguments>`
Connects to a local or online world