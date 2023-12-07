---
label: SetUp Portals
order: 99
icon: "/static/play.png"
---

<style>
    .sample {
        text-align: center;
        color: #1956AF;
        border-radius: 10px;
        background-color: #ff9500;
        border: 1px solid #1956AF;
        padding-top: 20px;
        margin-bottom: 20px;
    }
</style>


:::sample
Go to :  `Content/PortalTeleport/Blueprints/Portals/BP_LevelStreamerManager`
:::

# What is Level Streamer Manager?

The manager who is permanently located on the Base Level and controls the level transition portals and connects with the user interface.


`Starting Level` -> Load target level when game starting.

`Fade Speed` -> Level transition speed.


:::sample
Go to :  `Content/PortalTeleport/Blueprints/Portals/BP_LevelStreamerPortal`
:::

# What is Level Streamer Portal?

The portal who is load streaming level and located on the Base Level.


`Connected Level` -> Loading level.

`Connected Level Streamer` -> Target the level and portal.