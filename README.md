# Melon-PowerPlan-for-Windows
A custom made power plan for windows end user's to get the most out of thier pc's🍉

## About the powerplan
- maxed out everything even on battery power mode too *enable dc turbo boost from bios (for laptops)
- process states maxed out to 100% for no reason*😉


## whats inside 🍉Powerplan?
```bash
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
```

## How to use? Powerplan
- Download the latest [release](https://github.com/Nayemhasan/Hp_elitebook_840G5MAX/releases/tag/V.1)
- Run cmd as a administrator and type this
```bash
powercfg -import "the path of that config file"
```
- go to control panel and select the 🍉power plan and all set.
<p align="left">
  <img src="https://github.com/Nayemhasan/Hp_elitebook_840G5MAX/blob/main/Resources/powerplan.png">
</p>

- Done🍉
