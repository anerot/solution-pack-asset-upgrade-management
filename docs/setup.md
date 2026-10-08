| [Home](../README.md) |
|-----------------------------------------------------------------------------------------------------------------|

# Installation

1. To install a solution pack, click **Content Hub** > **Discover**.
2. From the list of solution packs that appears, search for and select **Asset Upgrade Management**.
3. Click the **Asset Upgrade Management** solution pack card.
4. Click **Install** on the bottom to begin the installation.

## Operation Modes
The Solution Pack operates either in:

- **Simulation Mode:** This mode allows you to run the "Start Group" playbook without adding Assets nor connector config in FortiSOAR and observe the User Input workflow. To turn demo mode on, you simply need to edit the `Start Group` playbook, edit the step `Configuration` and set the `UseMockOutput` variable to `true`.
- **Live Mode:** If you want to use the solution pack to handle your production Asset Upgrade, the above variable has to be set to `false`. Furthermore some prerequisites are required, the list is available under Prerequisites section of this document

## Prerequisites

The **Asset Upgrade Management** solution pack depends on the following connector that is installed automatically &ndash; if not already installed.

| Connector Name                | Purpose                                                             |
|:----------------------------------|:--------------------------------------------------------------------|
| Asset Upgrade                     | Required for Asset Upgrade Management                              |


### Prerequisites for Live Mode
- Demo mode turned off : `UseMockOutput` variable to `false`
- `Asset Upgrade` connector with as many configuration name as different username/password tuple to authenticate on your devices.
- The firmware file added as Attachment with `Type` defined as `Firmware`
- Assets in the Asset List

# Configuration

- The `Asset Upgrade` connector will store the username/password you will use to authenticate. If you use some different username/password for other devices then you have to create multiple `Configuration` in your connector. The Configuration name case is important and has to be the same than your Asset Config Name value.


# Next Steps
| [Usage](./usage.md) | [Contents](./contents.md) |
|---------------------|---------------------------|
