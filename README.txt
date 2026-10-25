FROST PLUGIN v2.8 + FROST RESOURCE PACK — MINECRAFT JAVA 1.21.11

TWO ZIP FILES:
- Frost_Resource_Pack_1.21.11.zip is installed in the Minecraft CLIENT resourcepacks folder.
- FrostPlugin_v2.8_Source.zip is Java source for your Paper SERVER plugin.

SERVER UPDATE (same GitHub method you've used before)
1. Upload source files from FrostPlugin_v2.8_Source.zip to your existing GitHub repository.
2. Your .github/workflows/build.yml can stay as it is. The ZIP also contains it.
3. Actions -> Build Frost Plugin -> Run workflow.
4. Download the artifact ZIP, extract the plugin .jar.
5. Stop your server and replace the previous Frost .jar with the new one. Restart.

CLIENT TEXTURES
1. Download Frost_Resource_Pack_1.21.11.zip; DO NOT extract.
2. Put it inside the Minecraft Java 1.21.11 resourcepacks directory.
3. Options -> Resource Packs -> enable Frost Resource Pack.
4. Join your Paper server; OPs can open /frost and obtain newly textured items.
5. To update Frost items ALREADY in your inventory: /frost reskin.
   That command preserves the item's enchantments, name, lore, and persistent data.
6. Normal vanilla items remain visually unchanged.

WORN ARMOR
Frozen equipment has a separate frosted equipment asset for the full worn armor set.
Diamond Rib trim is preserved by the plugin.

IMPORTANT
- Without the resource pack, the unique item_model IDs won't resolve and may show missing textures.
- This is a client-side resource pack; the plugin does NOT automatically send it to players.
  To distribute through your server later, host the ZIP and set resource-pack URL and SHA-1 in server.properties.
- This pack contains custom pixel-art sprites and JSON item models; it is not a 3D Blockbench model pack.
- Java source uses ItemMeta.setItemModel and EquippableComponent.setModel on Paper 1.21.11.
- The complete Paper API compilation/in-game rendering have not been run in this workspace.
- Resource pack format is 75 for Minecraft Java 1.21.11.
