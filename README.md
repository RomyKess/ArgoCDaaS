# ArgoCDaaS
This chart is designed to onboard new ArgoCD customers by only adding a values file tailored to them (names, sso groups, resources).
It allows you to create multi-project instances for clients who still want the advantages of sharing a single ArgoCD instance.
Some resources are part of the DR solution which is meant for restoring your instance including everything in it to a second cluster (limited with a sync window to disable a two-controllers situation).
The RBAC part is limiting the clients to only the necessary permissions needed, and non-clients to not be able to view anything.
Inclusions/Exclusions, Whitelists/Blacklists and destinations are also used to restrict the client resource-wise however you'd like.
