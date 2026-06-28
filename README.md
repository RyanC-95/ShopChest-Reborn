## ShopChest Reborn (WIP)

### ShopChest Reborn is currently in active development. While the core functionality is in place, there are still a number of known bugs and planned improvements. ShopChest Reborn has only been tested on Paper 26.1.2.

#

ShopChest Reborn is a modern, high-performance chest shop plugin for Paper servers, inspired by the original [ShopChest](https://www.spigotmc.org/resources/shopchest.11431/) and rebuilt from the ground up.

## New Features:

- **/shop find <item<item>>** will bring up a GUI with all shops in a configured radius (100 blocks) that are selling or buying that item. Click the shop to teleport to that shop

<img width="225" height="250" alt="2026-06-28_16 26 34" src="https://github.com/user-attachments/assets/6a8ef18d-9e5b-4f60-92ad-7b3f1778ddc9" />

<img width="225" height="250" alt="2026-06-28_16 20 13" src="https://github.com/user-attachments/assets/c4bd43e9-fc91-4691-8e2f-7aa564e946e9" />

<img width="225" height="250" alt="2026-06-28_16 26 58" src="https://github.com/user-attachments/assets/1ce5933c-8714-49f3-9c9d-2811decf19d7" />

<img width="289" height="21" alt="2026-06-28_16 32 15" src="https://github.com/user-attachments/assets/75a2a8c7-64ce-4792-823a-6a27800b7ed9" />

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

- Add shop creation fee and refund **[✔️]**
- Add configurable shop creation fees and refunds. **[✔️]**
- Add a configurable item blacklist. **[✔️]**
- Add protection to prevent blocks being placed above shop chests **[✔️]**
- Add allow-broken-items option **[✔️]**
- Prevent players from buying or selling while in Creative mode. **[✔️]**
- Configurable minimum/maximum prices and buy ≥ sell validation. **[❌]**
- Add decimal price support **[❌]**
- Add a configurable option to allow or disallow damaged items (items with durability loss) in shop transactions. **[❌]**
- Add a configurable tax system that deducts a percentage from every successful shop transaction. The tax should be configurable in config.yml and apply to both player shops and admin shops. **[❌]**
- Add shop owner (vendor) message notifications. **[❌]**
- Add a per-world shop creation toggle to config.yml, allowing server owners to enable or disable shop creation in specific worlds. **[❌]**
- Add Advanced Region Market hook so shops remove when region expires **[❌]**
- Add automatic invalid shop cleanup **[❌]**
- Add a **/shop limits** command that displays how many shops a player has created, their maximum shop limit, and how many remaining shops they can create. Add permission-based shop limits. **[❌]**
- Allow admins to run **/shop open** to view players shops **[❌]**
- Add a teleport delay **[❌]**
- Add configurable hologram view distance **[❌]**
- Add floating items above chest shops **[❌]**
- Add configurable floating item view distance **[❌]**
- Add "only show shops in sight" option **[❌]**
- Add a language file for item name translations **[❌]**
- Prevent players from creating a shop if there is a block directly above the shop container. **[❌]**


