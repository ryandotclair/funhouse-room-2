# cabinet-34

Continuous Deployment watch folder for the desk channel pin.

Put the desired state here. Let the cluster reconcile. That is the whole product
pitch. Touching files outside this directory is gossip, not delivery.

## Stage pin

`stage-config.yaml` is what the page reads after reconcile. Treat it like any
other desired-state file under Continuous Deployment.

The physical red console is not for editing this file by hand. It reverts the
**last production push** to the previous version (NKP Continuous Deployment
rollback). That is how Goon42 spends a Tuesday when he is bored.

Flux path is this directory only. If CD rolled you back and git looks dirty,
someone used the button. Ask around. Or don't. Plausible deniability is a
feature for some of us.
