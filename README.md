## ShopChest Reborn (WIP)

### ShopChest Reborn is currently in active development. While the core functionality is in place, there are still a number of known bugs and planned improvements. ShopChest Reborn has only been tested on Paper 26.1.2.

#

ShopChest Reborn is a modern, high-performance chest shop plugin for Paper servers, inspired by the original ShopChest and rebuilt from the ground up.

## New Features:

- **/shop find <item<item>>** will bring up a GUI with all shops in a configured radius (100 blocks) that are selling or buying that item. Click the shop to teleport to that shop
- Supports all container types as shops.
  - Chest
  - Ender Chest
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

## Roadmap
 **[❌]** = Not Done  
 **[✔️]** = Done  
 **[🐛]** = Bug
 
- Add a language file for item name translations **[❌]**
- Add Advanced Region Market hook so shops remove when region expires **[❌]**
- Allow admins to run **/shop open** to view players shops **[❌]**
- Add floating items above chest shops **[❌]**
- Prevent players from buying or selling while in Creative mode. **[❌]**
- Add a per-world shop creation toggle to config.yml, allowing server owners to enable or disable shop creation in specific worlds. **[❌]**
- Add a configurable tax system that deducts a percentage from every successful shop transaction. The tax should be configurable in config.yml and apply to both player shops and admin shops. **[❌]**
- Add a teleport delay **[❌]**
- Configurable minimum/maximum prices and buy ≥ sell validation. **[❌]**
- Add a **/shop limits** command that displays how many shops a player has created, their maximum shop limit, and how many remaining shops they can create. Add permission-based shop limits. **[❌]**
- Add a configurable option to allow or disallow damaged items (items with durability loss) in shop transactions. **[❌]**
- Add shop creation fee and refund **[✔️]**
- Add shop owner notifications **[❌]**
- Add "only show shops in sight" option **[❌]**
- Add decimal price support **[❌]**
- Add damaged item support **[❌]**
- Add automatic invalid shop cleanup **[❌]**
- Add configurable hologram view distance **[❌]**
- Add configurable floating item view distance **[❌]**
- Add a configurable item blacklist. **[✔️]**
- Add configurable shop creation fees and refunds. **[❌]**
- Add protection to prevent blocks being placed above shop chests **[🐛]** error in console
- Add shop owner (vendor) message notifications. **[❌]**


