## ShopChest Reborn (WIP)

### ShopChest Reborn is currently in active development. While the core functionality is in place, there are still a number of known bugs and planned improvements. ShopChest Reborn has only been tested on Paper 26.1.2.

#

ShopChest Reborn is a modern, high-performance chest shop plugin for Paper servers, inspired by the original [ShopChest](https://www.spigotmc.org/resources/shopchest.11431/) and rebuilt from the ground up.

## New Features:

- **/shop find <item<item>>** will bring up a GUI with all shops in a configured radius (100 blocks) that are selling or buying that item. Click the shop to teleport to that shop. Multi-word queries work: /shop find `oak planks` joins to `oak_planks`

<img width="196" height="192" alt="Buy" src="https://github.com/user-attachments/assets/b73d9a03-a8ab-499f-9e75-79d7ebd5edea" />

<img width="196" height="192" alt="Sell" src="https://github.com/user-attachments/assets/b1c030cb-8e90-4409-b4be-a21c48f3fead" />

<img width="196" height="192" alt="Buy   Sell" src="https://github.com/user-attachments/assets/f710ea82-de04-4823-9134-a726e7a3ffc3" />

<img width="196" height="192" alt="Admin Shop" src="https://github.com/user-attachments/assets/f5a266d7-1679-4f90-8f78-de9408023188" />

<img width="581" height="39" alt="Message" src="https://github.com/user-attachments/assets/273695a5-f0c4-41c7-bf63-13f20440c73e" />

- Supports all container types as shops.
  - Chest
  - Barrel 
  - Trapped Chest
  - Copper Chest
  - Exposed Copper Chest
  - Weathered Copper Chest
  - Oxidised Copper Chest
  - Waxed Copper Chest
  - Waxed Exposed Copper Chest
  - Waxed Weathered Copper Chest
  - Waxed Oxidised Copper Chest
- Added support for hex colours in hologram-format.yml.

## Commands
- /shop create <amount<amount>> <buy<buy>> <sell<sell>>
- /shop create <amount<amount>> <buy<buy>> <sell<sell>> admin
- /shop remove
- /shop info
- /shop open
- /shop find <item<item>>
- /shop reload
- /shop removeall <player<player>>
- /shop config
- /shop update

## Permissions

- shopchest.*
- shopchest.create
- shopchest.create.admin
- shopchest.create.protected
- shopchest.buy
- shopchest.sell
- shopchest.openOther
- shopchest.remove.other
- shopchest.remove.admin
- shopchest.reload
- shopchest.config
- shopchest.update
- shopchest.notification.update
- shopchest.find
- shopchest.find.teleport
- shopchest.bypass.blacklist
- shopchest.bypass.build-above

## Roadmap
 **[❌]** = Not Done  
 **[✔️]** = Done  
 **[🐛]** = Bug  
 **[💡]** = Considering

- Containers can still be used as shops even though they aren't on the "allowed-chest-types:" list **[🐛]**
- Add floating items above chest shops. Works, but is bugged **[🐛]**
- Players can create a shop if there is a block directly above the shop container. Bug fixed **[✔️]**
- Added WorldGuard ownership checks to prevent players from creating shops in regions they do not own. **[✔️]**
- Add configurable shop creation fees and refunds. **[✔️]**
- Add a configurable item blacklist. **[✔️]**
- Add protection to prevent blocks being placed above shop chests **[✔️]**
- Add allow-broken-items option **[✔️]**
- Prevent players from buying or selling while in Creative mode. **[✔️]**
- Configurable minimum/maximum prices and buy ≥ sell validation. **[✔️]**
  - Add per item minimum/maximum prices. **[❌]**
- Add decimal price support **[✔️]**
- Add a configurable tax system that deducts a percentage from every successful shop transaction. The tax should be configurable in config.yml and apply to both player shops and admin shops. **[✔️]**
- Add shop owner (vendor) message notifications. **[✔️]**
- Add a per-world shop creation toggle to config.yml, allowing server owners to enable or disable shop creation in specific worlds. **[✔️]**
- Automatically remove shops when a players region expires. **[✔️]**
- Add automatic invalid shop cleanup **[✔️]**
- Add a **/shop limits** command that displays how many shops a player has created, their maximum shop limit, and how many remaining shops they can create. Add permission-based shop limits. **[❌]**
- Allow admins to run **/shop open** to view players shops **[❌]**
- Add a teleport delay **[✔️]**
- Add configurable hologram view distance **[✔️]** *Optimise the hologram view distance system. It currently works, but it's too slow.*
- Add configurable floating item view distance **[❌]**
- Add "only show shops in sight" option **[✔️]**
- Add a language file for item name translations **[✔️]**
- Automatically reduce prices for inactive players' shops after a configurable number of days. **[💡]**
- Add a built-in transaction history viewer for shop owners that will open a GUI when they run command **/shop history**. Including who bought or sold items, the item, quantity, and price. **[💡]**

