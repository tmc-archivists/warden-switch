# Warden Switch Script

Hello. Today we will showcase a simple warden switch by Madman. This simple, five-minute build is able to completely disable the spawning of wardens from the activation of sculk shriekers. This can be used to easily loot ancient cities, without needing to worry about sneaking around sculk sensors.

This design relies on the mechanic that each player can only trigger a sculk shrieker every ten seconds. This device uses a player's arrow falling on an exactly 2.5 second interval to trigger the shrieker at the exact end of each cooldown, ensuring that the warden never spawns near the player. Since the warden attempts to spawn near the projectile and not the player, we can prevent them from spawning entirely by blocking all available spawning spaces within an 11x13x11 block cubic area. Since player projectiles take priority over the player themselves when activating sculk shriekers, we can ensure that a warden never spawns while the switch is active.

Here are all the materials necessary to build the warden switch. As you can see, these materials can easily fit in the player's inventory, using only three redstone components and eight temporary blocks.

[Block by block tutorial]

Now, for a few notes. The sculk shrieker must be naturally occurring, meaning it was previously generated in the world and not placed by a player. This is because player-placed shriekers have modified NBT data that does not allow them to spawn wardens. This device will only disable wardens for the owner of the arrow; however, other players can shoot their own arrows inside the machine as well to prevent warden spawning for them. It is advised to mine any sensors in the general area, place blocks (except the sensor), then flood, then place sensor at the very end just before firing arrows. You can cover the shrieker in wool while you mine sensors if you wish. It is also important to note that this will require chunk loading to function outside of the player's render distance. You can place an alternate account within render distance of the warden switch, or build a chunk loader, which is in the cards and the description.
