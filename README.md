# test-buildpacks-require-php


```
$ pack build myapp --buildpack ./php-detect --buildpack paketo-buildpacks/php-dist
jammy: Pulling from company/bitso-builder
Digest: sha256:33f5659cf306f3aa6a11493ff27563e556f1f83d34c601bf3fa633ded92aeccb
Status: Image is up to date for ghcr.io/company/bitso-builder:jammy
jammy: Pulling from company/bitso-runner
Digest: sha256:80e4bef10eee9531ee0202f4be8bfb1574aeb0438efdba55cbaa88576e1984fc
Status: Image is up to date for ghcr.io/company/bitso-runner:jammy
2.3.7: Pulling from paketo-buildpacks/php-dist
Digest: sha256:6583caaa8da02715c652c9daafabbbd60c3780fbcfae01fbbeaf2067c700afb5
Status: Image is up to date for gcr.io/paketo-buildpacks/php-dist:2.3.7
2.3.7: Pulling from paketo-buildpacks/php-dist
Digest: sha256:6583caaa8da02715c652c9daafabbbd60c3780fbcfae01fbbeaf2067c700afb5
Status: Image is up to date for gcr.io/paketo-buildpacks/php-dist:2.3.7
docker.io/paketobuildpacks/php-dist@sha256:6583caaa8da02715c652c9daafabbbd60c3780fbcfae01fbbeaf2067c700afb5: Pulling from paketobuildpacks/php-dist
Digest: sha256:6583caaa8da02715c652c9daafabbbd60c3780fbcfae01fbbeaf2067c700afb5
Status: Image is up to date for paketobuildpacks/php-dist@sha256:6583caaa8da02715c652c9daafabbbd60c3780fbcfae01fbbeaf2067c700afb5
docker.io/paketobuildpacks/php-dist@sha256:6583caaa8da02715c652c9daafabbbd60c3780fbcfae01fbbeaf2067c700afb5: Pulling from paketobuildpacks/php-dist
Digest: sha256:6583caaa8da02715c652c9daafabbbd60c3780fbcfae01fbbeaf2067c700afb5
Status: Image is up to date for paketobuildpacks/php-dist@sha256:6583caaa8da02715c652c9daafabbbd60c3780fbcfae01fbbeaf2067c700afb5
0.18.5: Pulling from buildpacksio/lifecycle
Digest: sha256:16a4c9e945381ad182fbb92710f0643e1c434ce11c3c43fb0ce6fcfce0d5efb7
Status: Image is up to date for buildpacksio/lifecycle:0.18.5
===> ANALYZING
[analyzer] Image with name "myapp" not found
===> DETECTING
[detector] ======== Results ========
[detector] pass: php-detect@0.0.1
[detector] pass: paketo-buildpacks/php-dist@2.3.7
[detector] Resolving plan... (try #1)
[detector] fail: php-detect@0.0.1 requires php
[detector] ERROR: No buildpack groups passed detection.
[detector] ERROR: Please check that you are running against the correct path.
[detector] ERROR: failed to detect: no buildpacks participating
ERROR: failed to build: executing lifecycle: failed with status code: 20
```