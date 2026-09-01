# SOMS Releases

Auto-published Windows installers for SOMS desktop. Do not commit manually.

Download: https://dolil.github.io/soms-releases/

The page links the latest Windows installer; older builds stay available on
the releases page.

It reads `latest.json`, which `.github/workflows/update-latest.yml` rewrites
from the newest published release on every release event. That file is
generated — don't hand-edit it. The page falls back to the GitHub API only if
`latest.json` is missing, because anonymous API callers share a quota of 60
requests an hour per IP address and get 403 for the rest of the hour once it
runs out — which used to break the page for everyone on that address.
