## Build and install
snapcraft pack
snapcraft install --dangerous psi-test*.snap

## Run Test
In console A
`snap run psi-test`

In console B (adjust vm-bytes to suit)
`stress-ng --vm 1 --vm-bytes 4G --timeout 60s`


Confirm PSI notifications received in console A when memory pressure is high.


