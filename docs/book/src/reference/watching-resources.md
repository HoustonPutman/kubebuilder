# Watching Resources

Inside a `Reconcile()` control loop, controllers will often use the state of the kubernetes cluster, and resources in it, to make decisions.
Therefore, it can be necessary to know when a resource that you care about is changed.

The [Controller Runtime libraries](https://pkg.go.dev/sigs.k8s.io/controller-runtime/pkg/builder) provide many ways for resources to be managed, and watched.
This ranges from the easy and obvious use cases, such as watching the resources you are controlling,
to more unique and advanced use cases.

See each subsection for explanations and examples of the different ways in which your controller can _Watch_ the resources it cares about.