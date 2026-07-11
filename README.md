<img width="1395" height="364" alt="ShopChest Reborn" src="https://github.com/user-attachments/assets/7c2972e5-141c-44f6-9a6b-e863c640422d" />

### ShopChest Reborn is currently in active development. While the core functionality is in place, there are still a number of known bugs and planned improvements. ShopChest Reborn has only been tested on Paper 26.1.2.

#

ShopChest Reborn is a modern, high-performance chest shop plugin, inspired by the original [ShopChest](https://www.spigotmc.org/resources/shopchest.11431/) and rebuilt from the ground up.

## New Features:

- **/shop find <item<item>>** will bring up a GUI with all shops in a configured radius (100 blocks) that are selling or buying that item. Click the shop to teleport to that shop. Multi-word queries work: /shop find `oak planks` joins to `oak_planks`

<img width="196" height="192" alt="Buy" src="https://github.com/user-attachments/assets/b73d9a03-a8ab-499f-9e75-79d7ebd5edea" />

<img width="196" height="192" alt="Sell" src="https://github.com/user-attachments/assets/b1c030cb-8e90-4409-b4be-a21c48f3fead" />

<img width="196" height="192" alt="Buy   Sell" src="https://github.com/user-attachments/assets/f710ea82-de04-4823-9134-a726e7a3ffc3" />

<img width="196" height="192" alt="Admin Shop" src="https://github.com/user-attachments/assets/f5a266d7-1679-4f90-8f78-de9408023188" />

<img width="608" height="52" alt="2026-07-06_11 01 13" src="https://github.com/user-attachments/assets/26e433de-4087-49a5-b4ff-4d3cc353cd41" />

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
 
Example of a Copper Chest Shop

<img width="722" height="437" alt="2026-07-10_18 25 53" src="https://github.com/user-attachments/assets/e2f9c4f0-cb28-4211-9ff9-d4ecce25e288" />

Example of automatic shop removal when you no longer own the region.

<img width="584" height="39" alt="2026-07-06_10 57 05 (1)" src="https://github.com/user-attachments/assets/557b5194-35ad-47a7-9466-1077c756da5e" />

Example of /shop info

<img width="452" height="146" alt="2026-07-04_13 20 05" src="https://github.com/user-attachments/assets/65e1bf91-9e09-436b-9a20-90c7a5854ee8" />

Example of per item tax

<img width="488" height="50" alt="Diamond" src="https://github.com/user-attachments/assets/978d7008-ae15-443e-83ed-71fc0babf9fe" />

<img width="488" height="50" alt="Emerald" src="https://github.com/user-attachments/assets/9ef0176e-f896-4725-9599-4b89bd14eaa2" />

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
- /shop limits
- /shop limits <player<player>>

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
- shopchest.limits
- shopchest.limits.other
- shopchest.limit.<X<X>> (e.g. shopchest.limit.5)
- shopchest.limit.*

## Roadmap
 **[🐛]** = Bug   
 **[❌]** = Not Done  
**[💡]** = Considering  
 **[✔️]** = Done  

##
- Holograms remain visible if another player is within the configured hologram view distance, even after I move out of range. Hologram visibility should be tracked per player, so each player only sees holograms while they are within the configured distance. [🐛]
- Floating item glitches when creating a shop with a barrel. The floating item does not stay above the shop and instead slides across the floor. [🐛]
- The %STOCK% placeholder in hologram-format.yml does not update when an admin adds items to a player's shop using /shop open. For example, I opened a player's bread shop with /shop open, placed 1 bread into the chest, but the hologram stock count did not update. The hologram should refresh immediately whenever the shop inventory changes, regardless of whether the owner or an admin modifies the inventory. [🐛]
##
- Hide commands in /shop if you don't have permission **[❌]**
- Display potion details (effects, duration, and level) in /shop info for potions. **[❌]**
##
- Automatically reduce prices for inactive players' shops after a configurable number of days. **[💡]**
- Add a built-in transaction history viewer for shop owners that will open a GUI when they run command **/shop history**. Including who bought or sold items, the item, quantity, and price. **[💡]**
- Add support for multiple currencies on admin shops, allowing each shop to use a configurable economy (e.g. Vault, PlayerPoints, Tokens). Example, /shop setcurrency playerpoints **[💡]**
##
- Add configurable hologram view distance **[✔️]**
  - *Optimise the hologram view distance system.* **[✔️]**
- Allow admins to run **/shop open** to view players shops **[✔️]** 
- Containers can still be used as shops even though they aren't on the "allowed-chest-types:" list. Bug fixed **[✔️]**
- Add floating items above chest shops. Bug fixed **[✔️]**
- Players can create a shop if there is a block directly above the shop container. Bug fixed **[✔️]**
- Added WorldGuard ownership checks to prevent players from creating shops in regions they do not own. **[✔️]**
- Add configurable shop creation fees and refunds. **[✔️]**
- Add a configurable item blacklist. **[✔️]**
- Add protection to prevent blocks being placed above shop chests **[✔️]**
- Add allow-broken-items option **[✔️]**
- Prevent players from buying or selling while in Creative mode. **[✔️]**
- Configurable minimum/maximum prices and buy ≥ sell validation. **[✔️]**
  - Add per item minimum/maximum prices. **[✔️]**
- Add decimal price support **[✔️]**
- Add a configurable tax system that deducts a percentage from every successful shop transaction. The tax should be configurable in config.yml and apply to both player shops and admin shops. **[✔️]**
  - Extend the tax system to support configurable per-item tax rates in a dedicated item-taxes.yml file. Each item can have its own buy and sell tax settings, overriding the global tax configuration where applicable. **[✔️]**
- Add shop owner (vendor) message notifications. **[✔️]**
  - Notify players of their offline shop earnings when they log in. **[✔️]**
- Add a per-world shop creation toggle to config.yml, allowing server owners to enable or disable shop creation in specific worlds. **[✔️]**
- Automatically remove shops when a players region expires. **[✔️]**
- Add automatic invalid shop cleanup **[✔️]**
- Add a teleport delay **[✔️]**
- Add "only show shops in sight" option **[✔️]**
- Add a language file for item name translations **[✔️]**
- Show enchantment information when hovering over enchanted items in /shop info. **[✔️]**
- Add a **/shop limits** command that displays how many shops a player has created, their maximum shop limit, and how many remaining shops they can create. Add permission-based shop limits. **[✔️]**

