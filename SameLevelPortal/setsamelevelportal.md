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
Go to :  `Content/PortalTeleport/Blueprints/Portals/BP_SameLevelPortal`
:::

# Add

-Drag it to your target level and set the scale to all axis `2`.

-Add another portal for connection with same settings


# Set

`Portal Render Quality` -> Portal render texture resolution.

`Connected Portal` -> Select target portal to go.

`Texture Render Target` -> Select different from the portal attached to the target tissue for processing.(if you stream on same time multiple portal you must choose different textures).

