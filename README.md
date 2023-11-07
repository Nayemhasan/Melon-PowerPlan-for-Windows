## Melon-PowerPlan-for-Windows🍉
A custom made power plan for windows end user's to get the most out of thier pc's & laptops. 
thanks to MICROSOFT <img src="https://commons.wikimedia.org/wiki/File:Microsoft_logo_(2012).svg#/media/File:Microsoft_logo_(2012).svg" alt="A beautiful landscape">



<p><a href="https://commons.wikimedia.org/wiki/File:Microsoft_logo_(2012).svg#/media/File:Microsoft_logo_(2012).svg"><img src="https://upload.wikimedia.org/wikipedia/commons/9/96/Microsoft_logo_%282012%29.svg" alt="Microsoft logo (2012).svg" height="109" width="512"></a><br>By &lt;a href="https://en.wikipedia.org/wiki/Microsoft" class="extiw" title="en:Microsoft"&gt;Microsoft Corporation&lt;/a&gt; - Jason Wells - &lt;a rel="nofollow" class="external text" href="https://info.flipgrid.com/"&gt;Flipgrid&lt;/a&gt; &lt;span style="font-size: 0.95em; font-weight: bold; color:#555; position: relative;"&gt;(in English)&lt;/span&gt;. &lt;a href="https://en.wikipedia.org/wiki/Microsoft" class="extiw" title="w:Microsoft"&gt;Microsoft&lt;/a&gt; (&lt;span class="mw-formatted-date" title="2018-06-18"&gt;June 18, 2018&lt;/span&gt;). Retrieved on &lt;span class="mw-formatted-date" title="2021-05-21"&gt;May 21, 2021&lt;/span&gt;. (&lt;a rel="nofollow" class="external text" href="https://static.flipgrid.com/fg-svgs/microsoft-logo.svg"&gt;Direct link&lt;/a&gt;)., Public Domain, <a href="https://commons.wikimedia.org/w/index.php?curid=20799781">Link</a></p>

<br>
<p align="left">
  <img src="https://img.shields.io/github/downloads/Nayemhasan/Melon-PowerPlan-for-Windows/total?style=social">
</p>

## About the powerplan⚡
- maxed out everything even on battery power mode too *enable dc turbo boost from bios (for laptops)
- process states maxed out to 100% for no reason*😉 & many more 
- now you can chose wether to use 100% cpu all the time or not with these 2 new powerplans (MelonV3+UltimateMelonV3)
- MelonV3 provides outsanding performance respected to thermals - cpu_idle support
<p align="left">
  <img src="https://github.com/Nayemhasan/Melon-PowerPlan-for-Windows/blob/main/pics/v3.png">
</p>

- UltimateMelonV3 provides maxed-out everything for hardcore users - no cpu_idle *make sure proper cooling
<p align="left">
  <img src="https://github.com/Nayemhasan/Melon-PowerPlan-for-Windows/blob/main/pics/v3ultimate.png">
</p>

<br>

## Whats inside 🍉Powerplan?

<details>
<summary>power scheme summary for desktop & laptop</summary>

```bash
# Configure power plan settings for desktops
$desktopSettingsCommands = @(
    "powercfg -setacvalueindex $guid SUB_PROCESSOR PROCTHROTTLEMAX 100",
    "powercfg -setacvalueindex $guid SUB_PROCESSOR PROCTHROTTLEMIN 100",
    "powercfg -setacvalueindex $guid SUB_PROCESSOR PROCTHROTTLEPCT 100",
    "powercfg -setacvalueindex $guid SUB_BUTTONS POWERBUTTONACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS SLEEPBUTTONACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS LIDOPENPOWERBUTTONACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS POWERBUTTONACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS SLEEPBUTTONACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS LIDOPENPOWERBUTTONACTION 0"
)

# Configure power plan settings for laptops
$laptopSettingsCommands = @(
    "powercfg -setacvalueindex $guid SUB_VIDEO VIDEOIDLE 0",
    "powercfg -setacvalueindex $guid SUB_VIDEO BRIGHTNESS 100",
    "powercfg -setacvalueindex $guid SUB_BUTTONS LIDACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS LIDCLOSEACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS POWERBUTTONACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS SLEEPBUTTONACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS LIDOPENPOWERBUTTONACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS POWERBUTTONACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS SLEEPBUTTONACTION 0",
    "powercfg -setacvalueindex $guid SUB_BUTTONS LIDOPENPOWERBUTTONACTION 0",
    "powercfg -setacvalueindex $guid SUB_PROCESSOR PROCTHROTTLEMAX 100",
    "powercfg -setacvalueindex $guid SUB_PROCESSOR PROCTHROTTLEMIN 100",
    "powercfg -setacvalueindex $guid SUB_PROCESSOR PROCTHROTTLEPCT 100"
)
```
</details>


<details>
<summary>contents of MelonV3 power scheme</summary>

```
Power Scheme GUID: 9712253e-f58d-4b9a-a12b-70463d94d896  (MelonV3)
  Subgroup GUID: 0012ee47-9041-4b5d-9b77-535fba8b1442  (Hard disk)
    GUID Alias: SUB_DISK
    Power Setting GUID: 6738e2c4-e8a5-4a42-b16a-e040e769756e  (Turn off hard disk after)
      GUID Alias: DISKIDLE
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0xffffffff
      Possible Settings increment: 0x00000001
      Possible Settings units: Seconds
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x000004b0

  Subgroup GUID: 0d7dbae2-4294-402a-ba8e-26777e8488cd  (Desktop background settings)
    Power Setting GUID: 309dce9b-bef4-4119-9921-a851fb12f0f4  (Slide show)
      Possible Setting Index: 000
      Possible Setting Friendly Name: Available
      Possible Setting Index: 001
      Possible Setting Friendly Name: Paused
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

  Subgroup GUID: 19cbb8fa-5279-450e-9fac-8a3d5fedd0c1  (Wireless Adapter Settings)
    Power Setting GUID: 12bbebe6-58d6-4636-95bb-3217ef867c1a  (Power Saving Mode)
      Possible Setting Index: 000
      Possible Setting Friendly Name: Maximum Performance
      Possible Setting Index: 001
      Possible Setting Friendly Name: Low Power Saving
      Possible Setting Index: 002
      Possible Setting Friendly Name: Medium Power Saving
      Possible Setting Index: 003
      Possible Setting Friendly Name: Maximum Power Saving
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

  Subgroup GUID: 238c9fa8-0aad-41ed-83f4-97be242c8f20  (Sleep)
    GUID Alias: SUB_SLEEP
    Power Setting GUID: 29f6c1db-86da-48c5-9fdb-f2b67b1f44da  (Sleep after)
      GUID Alias: STANDBYIDLE
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0xffffffff
      Possible Settings increment: 0x00000001
      Possible Settings units: Seconds
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

    Power Setting GUID: 94ac6d29-73ce-41a6-809f-6363ba21b47e  (Allow hybrid sleep)
      GUID Alias: HYBRIDSLEEP
      Possible Setting Index: 000
      Possible Setting Friendly Name: Off
      Possible Setting Index: 001
      Possible Setting Friendly Name: On
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000001

    Power Setting GUID: 9d7815a6-7ee4-497e-8888-515a05f02364  (Hibernate after)
      GUID Alias: HIBERNATEIDLE
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0xffffffff
      Possible Settings increment: 0x00000001
      Possible Settings units: Seconds
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

    Power Setting GUID: bd3b718a-0680-4d9d-8ab2-e1d2b4ac806d  (Allow wake timers)
      GUID Alias: RTCWAKE
      Possible Setting Index: 000
      Possible Setting Friendly Name: Disable
      Possible Setting Index: 001
      Possible Setting Friendly Name: Enable
      Possible Setting Index: 002
      Possible Setting Friendly Name: Important Wake Timers Only
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

  Subgroup GUID: 2a737441-1930-4402-8d77-b2bebba308a3  (USB settings)
    Power Setting GUID: 48e6b7a6-50f5-4782-a5d4-53bb8f07e226  (USB selective suspend setting)
      Possible Setting Index: 000
      Possible Setting Friendly Name: Disabled
      Possible Setting Index: 001
      Possible Setting Friendly Name: Enabled
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000001

  Subgroup GUID: 4f971e89-eebd-4455-a8de-9e59040e7347  (Power buttons and lid)
    GUID Alias: SUB_BUTTONS
    Power Setting GUID: a7066653-8d6c-40a8-910e-a1f54b84c7e5  (Start menu power button)
      GUID Alias: UIBUTTON_ACTION
      Possible Setting Index: 000
      Possible Setting Friendly Name: Sleep
      Possible Setting Index: 001
      Possible Setting Friendly Name: Hibernate
      Possible Setting Index: 002
      Possible Setting Friendly Name: Shut down
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

  Subgroup GUID: 501a4d13-42af-4429-9fd1-a8218c268e20  (PCI Express)
    GUID Alias: SUB_PCIEXPRESS
    Power Setting GUID: ee12f906-d277-404b-b6da-e5fa1a576df5  (Link State Power Management)
      GUID Alias: ASPM
      Possible Setting Index: 000
      Possible Setting Friendly Name: Off
      Possible Setting Index: 001
      Possible Setting Friendly Name: Moderate power savings
      Possible Setting Index: 002
      Possible Setting Friendly Name: Maximum power savings
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

  Subgroup GUID: 54533251-82be-4824-96c1-47b60b740d00  (Processor power management)
    GUID Alias: SUB_PROCESSOR
    Power Setting GUID: 5d76a2ca-e8c0-402f-a133-2158492d58ad  (Processor idle disable)
      GUID Alias: IDLEDISABLE
      Possible Setting Index: 000
      Possible Setting Friendly Name: Enable idle
      Possible Setting Index: 001
      Possible Setting Friendly Name: Disable idle
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

    Power Setting GUID: 893dee8e-2bef-41e0-89c6-b55d0929964c  (Minimum processor state)
      GUID Alias: PROCTHROTTLEMIN
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000064
    Current DC Power Setting Index: 0x00000005

    Power Setting GUID: 94d3a615-a899-4ac5-ae2b-e4d8f634367f  (System cooling policy)
      GUID Alias: SYSCOOLPOL
      Possible Setting Index: 000
      Possible Setting Friendly Name: Passive
      Possible Setting Index: 001
      Possible Setting Friendly Name: Active
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000001

    Power Setting GUID: bc5038f7-23e0-4960-96da-33abaf5935ec  (Maximum processor state)
      GUID Alias: PROCTHROTTLEMAX
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000064
    Current DC Power Setting Index: 0x00000064

  Subgroup GUID: 7516b95f-f776-4464-8c53-06167f40cc99  (Display)
    GUID Alias: SUB_VIDEO
    Power Setting GUID: 3c0bc021-c8a8-4e07-a973-6b14cbcb2b7e  (Turn off display after)
      GUID Alias: VIDEOIDLE
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0xffffffff
      Possible Settings increment: 0x00000001
      Possible Settings units: Seconds
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000258

    Power Setting GUID: aded5e82-b909-4619-9949-f5d71dac0bcb  (Display brightness)
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000064
    Current DC Power Setting Index: 0x00000064

    Power Setting GUID: f1fbfde2-a960-4165-9f88-50667911ce96  (Dimmed display brightness)
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000032
    Current DC Power Setting Index: 0x00000032

    Power Setting GUID: fbd9aa66-9553-4097-ba44-ed6e9d65eab8  (Enable adaptive brightness)
      GUID Alias: ADAPTBRIGHT
      Possible Setting Index: 000
      Possible Setting Friendly Name: Off
      Possible Setting Index: 001
      Possible Setting Friendly Name: On
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

  Subgroup GUID: 9596fb26-9850-41fd-ac3e-f7c3c00afd4b
    Power Setting GUID: 10778347-1370-4ee0-8bbd-33bdacaade49  (Video playback quality bias)
      Possible Setting Index: 000
      Possible Setting Friendly Name: Video playback power-saving bias
      Possible Setting Index: 001
      Possible Setting Friendly Name: Video playback performance bias
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000000

    Power Setting GUID: 34c7b99f-9a6d-4b3c-8dc7-b6693b78cef4  (When playing video)
      Possible Setting Index: 000
      Possible Setting Friendly Name: Optimise video quality
      Possible Setting Index: 001
      Possible Setting Friendly Name: Balanced
      Possible Setting Index: 002
      Possible Setting Friendly Name: Optimise power savings
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

  Subgroup GUID: e73a048d-bf27-4f12-9731-8b2076e8891f  (Battery)
    GUID Alias: SUB_BATTERY
    Power Setting GUID: 5dbb7c9f-38e9-40d2-9749-4f8a0e9f640f  (Critical battery notification)
      GUID Alias: BATFLAGSCRIT
      Possible Setting Index: 000
      Possible Setting Friendly Name: Off
      Possible Setting Index: 001
      Possible Setting Friendly Name: On
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000001

    Power Setting GUID: 637ea02f-bbcb-4015-8e2c-a1c7b9c0b546  (Critical battery action)
      GUID Alias: BATACTIONCRIT
      Possible Setting Index: 000
      Possible Setting Friendly Name: Do nothing
      Possible Setting Index: 001
      Possible Setting Friendly Name: Sleep
      Possible Setting Index: 002
      Possible Setting Friendly Name: Hibernate
      Possible Setting Index: 003
      Possible Setting Friendly Name: Shut down
    Current AC Power Setting Index: 0x00000002
    Current DC Power Setting Index: 0x00000002

    Power Setting GUID: 8183ba9a-e910-48da-8769-14ae6dc1170a  (Low battery level)
      GUID Alias: BATLEVELLOW
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x0000000a
    Current DC Power Setting Index: 0x0000000a

    Power Setting GUID: 9a66d8d7-4ff7-4ef9-b5a2-5a326ca2a469  (Critical battery level)
      GUID Alias: BATLEVELCRIT
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000005
    Current DC Power Setting Index: 0x00000005

    Power Setting GUID: bcded951-187b-4d05-bccc-f7e51960c258  (Low battery notification)
      GUID Alias: BATFLAGSLOW
      Possible Setting Index: 000
      Possible Setting Friendly Name: Off
      Possible Setting Index: 001
      Possible Setting Friendly Name: On
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000001

    Power Setting GUID: d8742dcb-3e6a-4b3c-b3fe-374623cdcf06  (Low battery action)
      GUID Alias: BATACTIONLOW
      Possible Setting Index: 000
      Possible Setting Friendly Name: Do nothing
      Possible Setting Index: 001
      Possible Setting Friendly Name: Sleep
      Possible Setting Index: 002
      Possible Setting Friendly Name: Hibernate
      Possible Setting Index: 003
      Possible Setting Friendly Name: Shut down
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

    Power Setting GUID: f3c5027d-cd16-4930-aa6b-90db844a8f00  (Reserve battery level)
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000007
    Current DC Power Setting Index: 0x00000007

```

</details>


<details>
<summary>contents of UltimateMelonV3 power scheme</summary>

```
Power Scheme GUID: 61e60280-bca9-439e-955a-a5c23faa20e6  (UltimateMelonV3)
  Subgroup GUID: 0012ee47-9041-4b5d-9b77-535fba8b1442  (Hard disk)
    GUID Alias: SUB_DISK
    Power Setting GUID: 6738e2c4-e8a5-4a42-b16a-e040e769756e  (Turn off hard disk after)
      GUID Alias: DISKIDLE
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0xffffffff
      Possible Settings increment: 0x00000001
      Possible Settings units: Seconds
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

  Subgroup GUID: 0d7dbae2-4294-402a-ba8e-26777e8488cd  (Desktop background settings)
    Power Setting GUID: 309dce9b-bef4-4119-9921-a851fb12f0f4  (Slide show)
      Possible Setting Index: 000
      Possible Setting Friendly Name: Available
      Possible Setting Index: 001
      Possible Setting Friendly Name: Paused
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000001

  Subgroup GUID: 19cbb8fa-5279-450e-9fac-8a3d5fedd0c1  (Wireless Adapter Settings)
    Power Setting GUID: 12bbebe6-58d6-4636-95bb-3217ef867c1a  (Power Saving Mode)
      Possible Setting Index: 000
      Possible Setting Friendly Name: Maximum Performance
      Possible Setting Index: 001
      Possible Setting Friendly Name: Low Power Saving
      Possible Setting Index: 002
      Possible Setting Friendly Name: Medium Power Saving
      Possible Setting Index: 003
      Possible Setting Friendly Name: Maximum Power Saving
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000002

  Subgroup GUID: 238c9fa8-0aad-41ed-83f4-97be242c8f20  (Sleep)
    GUID Alias: SUB_SLEEP
    Power Setting GUID: 29f6c1db-86da-48c5-9fdb-f2b67b1f44da  (Sleep after)
      GUID Alias: STANDBYIDLE
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0xffffffff
      Possible Settings increment: 0x00000001
      Possible Settings units: Seconds
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000384

    Power Setting GUID: 94ac6d29-73ce-41a6-809f-6363ba21b47e  (Allow hybrid sleep)
      GUID Alias: HYBRIDSLEEP
      Possible Setting Index: 000
      Possible Setting Friendly Name: Off
      Possible Setting Index: 001
      Possible Setting Friendly Name: On
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000001

    Power Setting GUID: 9d7815a6-7ee4-497e-8888-515a05f02364  (Hibernate after)
      GUID Alias: HIBERNATEIDLE
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0xffffffff
      Possible Settings increment: 0x00000001
      Possible Settings units: Seconds
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

    Power Setting GUID: bd3b718a-0680-4d9d-8ab2-e1d2b4ac806d  (Allow wake timers)
      GUID Alias: RTCWAKE
      Possible Setting Index: 000
      Possible Setting Friendly Name: Disable
      Possible Setting Index: 001
      Possible Setting Friendly Name: Enable
      Possible Setting Index: 002
      Possible Setting Friendly Name: Important Wake Timers Only
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000000

  Subgroup GUID: 2a737441-1930-4402-8d77-b2bebba308a3  (USB settings)
    Power Setting GUID: 48e6b7a6-50f5-4782-a5d4-53bb8f07e226  (USB selective suspend setting)
      Possible Setting Index: 000
      Possible Setting Friendly Name: Disabled
      Possible Setting Index: 001
      Possible Setting Friendly Name: Enabled
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000001

  Subgroup GUID: 4f971e89-eebd-4455-a8de-9e59040e7347  (Power buttons and lid)
    GUID Alias: SUB_BUTTONS
    Power Setting GUID: a7066653-8d6c-40a8-910e-a1f54b84c7e5  (Start menu power button)
      GUID Alias: UIBUTTON_ACTION
      Possible Setting Index: 000
      Possible Setting Friendly Name: Sleep
      Possible Setting Index: 001
      Possible Setting Friendly Name: Hibernate
      Possible Setting Index: 002
      Possible Setting Friendly Name: Shut down
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

  Subgroup GUID: 501a4d13-42af-4429-9fd1-a8218c268e20  (PCI Express)
    GUID Alias: SUB_PCIEXPRESS
    Power Setting GUID: ee12f906-d277-404b-b6da-e5fa1a576df5  (Link State Power Management)
      GUID Alias: ASPM
      Possible Setting Index: 000
      Possible Setting Friendly Name: Off
      Possible Setting Index: 001
      Possible Setting Friendly Name: Moderate power savings
      Possible Setting Index: 002
      Possible Setting Friendly Name: Maximum power savings
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000002

  Subgroup GUID: 54533251-82be-4824-96c1-47b60b740d00  (Processor power management)
    GUID Alias: SUB_PROCESSOR
    Power Setting GUID: 5d76a2ca-e8c0-402f-a133-2158492d58ad  (Processor idle disable)
      GUID Alias: IDLEDISABLE
      Possible Setting Index: 000
      Possible Setting Friendly Name: Enable idle
      Possible Setting Index: 001
      Possible Setting Friendly Name: Disable idle
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000000

    Power Setting GUID: 893dee8e-2bef-41e0-89c6-b55d0929964c  (Minimum processor state)
      GUID Alias: PROCTHROTTLEMIN
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000064
    Current DC Power Setting Index: 0x00000005

    Power Setting GUID: 94d3a615-a899-4ac5-ae2b-e4d8f634367f  (System cooling policy)
      GUID Alias: SYSCOOLPOL
      Possible Setting Index: 000
      Possible Setting Friendly Name: Passive
      Possible Setting Index: 001
      Possible Setting Friendly Name: Active
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000000

    Power Setting GUID: bc5038f7-23e0-4960-96da-33abaf5935ec  (Maximum processor state)
      GUID Alias: PROCTHROTTLEMAX
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000064
    Current DC Power Setting Index: 0x00000064

  Subgroup GUID: 7516b95f-f776-4464-8c53-06167f40cc99  (Display)
    GUID Alias: SUB_VIDEO
    Power Setting GUID: 3c0bc021-c8a8-4e07-a973-6b14cbcb2b7e  (Turn off display after)
      GUID Alias: VIDEOIDLE
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0xffffffff
      Possible Settings increment: 0x00000001
      Possible Settings units: Seconds
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x0000012c

    Power Setting GUID: aded5e82-b909-4619-9949-f5d71dac0bcb  (Display brightness)
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000064
    Current DC Power Setting Index: 0x00000028

    Power Setting GUID: f1fbfde2-a960-4165-9f88-50667911ce96  (Dimmed display brightness)
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000032
    Current DC Power Setting Index: 0x00000032

    Power Setting GUID: fbd9aa66-9553-4097-ba44-ed6e9d65eab8  (Enable adaptive brightness)
      GUID Alias: ADAPTBRIGHT
      Possible Setting Index: 000
      Possible Setting Friendly Name: Off
      Possible Setting Index: 001
      Possible Setting Friendly Name: On
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

  Subgroup GUID: 9596fb26-9850-41fd-ac3e-f7c3c00afd4b
    Power Setting GUID: 10778347-1370-4ee0-8bbd-33bdacaade49  (Video playback quality bias)
      Possible Setting Index: 000
      Possible Setting Friendly Name: Video playback power-saving bias
      Possible Setting Index: 001
      Possible Setting Friendly Name: Video playback performance bias
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000000

    Power Setting GUID: 34c7b99f-9a6d-4b3c-8dc7-b6693b78cef4  (When playing video)
      Possible Setting Index: 000
      Possible Setting Friendly Name: Optimise video quality
      Possible Setting Index: 001
      Possible Setting Friendly Name: Balanced
      Possible Setting Index: 002
      Possible Setting Friendly Name: Optimise power savings
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000001

  Subgroup GUID: e73a048d-bf27-4f12-9731-8b2076e8891f  (Battery)
    GUID Alias: SUB_BATTERY
    Power Setting GUID: 5dbb7c9f-38e9-40d2-9749-4f8a0e9f640f  (Critical battery notification)
      GUID Alias: BATFLAGSCRIT
      Possible Setting Index: 000
      Possible Setting Friendly Name: Off
      Possible Setting Index: 001
      Possible Setting Friendly Name: On
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000001

    Power Setting GUID: 637ea02f-bbcb-4015-8e2c-a1c7b9c0b546  (Critical battery action)
      GUID Alias: BATACTIONCRIT
      Possible Setting Index: 000
      Possible Setting Friendly Name: Do nothing
      Possible Setting Index: 001
      Possible Setting Friendly Name: Sleep
      Possible Setting Index: 002
      Possible Setting Friendly Name: Hibernate
      Possible Setting Index: 003
      Possible Setting Friendly Name: Shut down
    Current AC Power Setting Index: 0x00000002
    Current DC Power Setting Index: 0x00000002

    Power Setting GUID: 8183ba9a-e910-48da-8769-14ae6dc1170a  (Low battery level)
      GUID Alias: BATLEVELLOW
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x0000000a
    Current DC Power Setting Index: 0x0000000a

    Power Setting GUID: 9a66d8d7-4ff7-4ef9-b5a2-5a326ca2a469  (Critical battery level)
      GUID Alias: BATLEVELCRIT
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000005
    Current DC Power Setting Index: 0x00000005

    Power Setting GUID: bcded951-187b-4d05-bccc-f7e51960c258  (Low battery notification)
      GUID Alias: BATFLAGSLOW
      Possible Setting Index: 000
      Possible Setting Friendly Name: Off
      Possible Setting Index: 001
      Possible Setting Friendly Name: On
    Current AC Power Setting Index: 0x00000001
    Current DC Power Setting Index: 0x00000001

    Power Setting GUID: d8742dcb-3e6a-4b3c-b3fe-374623cdcf06  (Low battery action)
      GUID Alias: BATACTIONLOW
      Possible Setting Index: 000
      Possible Setting Friendly Name: Do nothing
      Possible Setting Index: 001
      Possible Setting Friendly Name: Sleep
      Possible Setting Index: 002
      Possible Setting Friendly Name: Hibernate
      Possible Setting Index: 003
      Possible Setting Friendly Name: Shut down
    Current AC Power Setting Index: 0x00000000
    Current DC Power Setting Index: 0x00000000

    Power Setting GUID: f3c5027d-cd16-4930-aa6b-90db844a8f00  (Reserve battery level)
      Minimum Possible Setting: 0x00000000
      Maximum Possible Setting: 0x00000064
      Possible Settings increment: 0x00000001
      Possible Settings units: %
    Current AC Power Setting Index: 0x00000007
    Current DC Power Setting Index: 0x00000007

```

</details>
<br>

## How to use?🍉Powerplan
- Download the latest [release](https://github.com/Nayemhasan/Melon-PowerPlan-for-Windows/releases)
- Run cmd as a administrator and type this
```bash
powercfg -import "the path of that config file"
```
<p align="left">
  <img src="https://github.com/Nayemhasan/Melon-PowerPlan-for-Windows/blob/main/pics/path.png">
</p>

- Go to control panel and select the preferred one.
<p align="left">
  <img src="https://github.com/Nayemhasan/Melon-PowerPlan-for-Windows/blob/main/pics/def.png">
</p>

- Done🍉

## Bonus tips:

want more pow? try these 🔻

turn off : transparency effects from colors settings

turn off : fast startup(*for more stable system)

want more fps?: turn off gpu audio output from nvidia/amd gpu control panel

additionally: you can turn off page files from System Properties & speed up your ssd using [melonbooster🍉🔥](https://github.com/watermelonvault/Melon_booster)






