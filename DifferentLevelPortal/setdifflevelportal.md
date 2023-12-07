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
Go to :  `Content/PortalTeleport/Blueprints/Portals/BP_DiffLevelPortalTunnel`
:::

# Add

-Open a created sublevel

-Drag it to your target level and set the scale to all axis `2`.

-Open another created sublevel for portal connection

-Add another portal for connection with same settings


# Set

`Tag` -> Unique Tag of portal for runtime connection.

`Target Tag` -> Find target portal with Tag in loaded level.

`Connected Level` -> The upload target level of the portal.

`Portal Render Quality` ->  Portal render texture resolution.

`Connected Portal` -> [Do not select].Is auto fill.

`Texture Render Target` -> Select different from the portal attached to the target tissue for processing.(if you stream on same time multiple portal you must choose different textures).


:::sample
Go to :  `Content/PortalTeleport/Blueprints/Portals/BP_LightChannelTrigger`
:::

# Multiple Directional Light Setup

When we load two levels at the same time and they have different directional light sources, these lights may overlap and distort the lighting, so it needs to be adjusted.

 If you do not use a directional light source per level, this setting is unimportant.

 -On the base level set up select SkyAtmosphere and set height `1` for reflection dont affect level meshs.

 -Changing a Directional light channel can be effect your main character for this issue you can add BP_LightChannelTrigger on the  location of level start/spawn point and set channel for auto setup.

 ::

    Open First level
    Select your Directional light
    In Detail panel search `Channel`
    Select a Channel
    Make the channel settings of the meshes of all models in the level the same
    On the portal location add BP_LightChannelTrigger and set up the scale
    In BP_LightChannelTrigger detail set the light channel section
    You can also assign the Directional light for auto set forward shading priority
    Open Second level
    Repeat all step but with different channel

 ::