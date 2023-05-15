## Description 

This is a test for the ConfigMap Resource. It checks if the resource has a label in its metadata or not.

## Expected Behavior

The ConfigMaps with namespace belonging with **team-\*** (reges) should be mutated so that if it doesn't have any labels associated with it, then the following label will be added to its metadata.
`lfx-mentorship: kyverno`. If this occurs, the test passes. If not, then the test fails. 

## Reference Issue(s)

N/A