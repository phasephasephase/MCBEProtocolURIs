# List of Minecraft: Bedrock Edition URI protocol links

All of these links were gathered by reverse engineering the latest Windows client binary (1.21.2 at the time). **Prefix each with `minecraft://`.**

## `?showHowToPlayScreen=1`

Shows the how to play screen

## `oculus_launched <no arguments>`

A shortcut to the game for Oculus (VR) users

## `?addExternalServer=<server name: string>|<ip: string>:<port: number>`

Adds an external server to the server list

## `?showStoreOffer=<item: UUID>`

Shows an item on the marketplace

## `?showOfferCollection=<document/page ID>`

Shows a specific Marketplace document or page. The `document/page ID` parameter should be the identifier of the document/page you want to open.

Examples:

- To open a specific page in the Marketplace: `minecraft://?showOfferCollection=MultiItemPage_PersonaCharacterCreator`

- To open the root page of the Marketplace: `minecraft://?showOfferCollection=marketplace?pageId=MultiItemPage_StoreRoot`

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

## `connectToRealm?realmId=<realm id: string> OR inviteID=<realm invite code: string>`

Connects to a Realm

## `?slashcommand=<command: string>`

Executes a command in the current server. This will disconnect the user if used in a local world.

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

Connects to a local world by its locally stored ID

## `connect/?<many arguments>`

Connects to a local or online world. Possible arguments are as follows:

### `localLevelId=<local level id: string>`

Acts similarly to `?load`

### `localWorld=<world name: string>`

Connects to a world by its name

### `serverUrl=<ip: string>`

Address of the server to connect to. If `?serverPort` is not specified, it will be 19132.

### `serverPort=<port: number>`

Port of the server to connect to. Must be used with `?serverUrl`
