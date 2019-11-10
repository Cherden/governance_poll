# Governance System
This rell module creates polls to let your users govern your dapp. Each user has a balance of "poll tokens" which can be used as votes. In our use-case, users will be able to balance stats for characters in our game.

## Integration
The module specifies includes a file `governance/interface.rell`. There, functions are defined which allow you to interact with the module. In general, you only have to adjust this file.

To adjust the module to your dapp, use the `Parameters` object.

At the end of the interface file, there are `check_on` functions defined. Use those to add extra checks before a vote or poll is created. The comment blocks before the functions indicate what conditions are already handled inside the system.

An example on how to use the module can be found in `main.rell`.