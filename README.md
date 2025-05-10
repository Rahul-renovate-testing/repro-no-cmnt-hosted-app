### Test details

This repo contains a `renovate/reconfigure` branch which has invalid renovate config.
There's a PR created using the reconfigure branch.

Expected: The bot finds the reconfigure PR and adds a comment informing the user about the invalid config

Actual outcome: The bot cannot finf the reconfigure PR

<details>
  <summary>Related Logs</summary>

```
DEBUG: findPr(renovate/reconfigure, undefined, open)
DEBUG: http cache: saving https://api.github.com/repos/Rahul-renovate-testing/repro-no-cmnt-hosted-app/pulls?head=Rahul-renovate-testing/repro-no-cmnt-hosted-app:renovate/reconfigure&state=open (etag="77783e03fba4adc74bcb90b7ec4d3d30e1babd1d821923c511fb643e4845fc4c", lastModified=undefined)
DEBUG: No PR found for branch renovate/reconfigure
```
</details>
