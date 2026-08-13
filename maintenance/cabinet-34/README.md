# cabinet-34

Continuous Deployment watch folder for the desk channel service.

Put the desired state here. Let the cluster reconcile. That is the whole product
pitch. Touching files outside this directory is gossip, not delivery.

Flux owns Deployment, Service, and IngressRoute in this directory. Runtime stage
env (which build the desk page thinks it is) lives in a ConfigMap the night
console mutates. It is **not** in this repo on purpose. If you are grepping for
`STAGE:` here, you are looking at the wrong control plane.

The physical red console reverts the **last production push** to the previous
version (NKP Continuous Deployment rollback).

If CD rolled you back and your laptop still shows the old page, roll the desk
pods or ask who was near the button. Plausible deniability is a feature for
some of us.
