## Instant Website - Infrastructure
> Good ol' ssh-based infrastructure.

### Overview

Since we're not doing anything remotely complex here, we try to keep it as simple
as possible. That means, no containers, no extra runtimes needed, no fancy stuff
at all. You change a file here, then you SCP it over, restart the appropriate
service and you're done.

If we need something fancier in the future, we'll setup something fancier. For
now this works fine for the scale we're dealing with.

#### Location of stuff

- Nameservers + DNS records with CloudFlare for now
- Dedicated host at Hetzner
- Domain owned by account in Gandi

- InstantWebsite jar file run by systemd
- Caddy acts as front for entire host
- Just one machine until we need more. Scale with fatter host before adding more hosts

## License

Copyright 2020 - Instant Website
