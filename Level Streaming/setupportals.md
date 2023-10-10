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
Go to :  `Content/Teleport/Blueprint/BP_LevelStreamer`
:::


# What is Level Streamer?

The level it connects to and the portal/level it will go to
When used to hold references, it frees up the level it is connected to from the level publisher, freeing up space for RAM and rendering, and provides a smooth transition by loading the targeted portal/level from the front.


`Connected Level` -> It is the level it is in and will close when used.

`Connected Level Streamer` -> Specifies the level and portal to go to.
