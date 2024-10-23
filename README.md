#  AWF Zephyr

Repository to setup Zephyr (sendrato-fork) to build `awareable-fw/apps`.

The following repositories will be fetched:
- `zephyr`: Sendrato's fork of Zephyr OS containing custom QN9090 soc definition.
- `awareable-fw`: Awareable-stack.
- `ol23_sdk`: SynchronicIT SDK used to build applications for the NXP OL23.
- `nrf`: Sendrato's fork of NCS (nRF Connect SDK), used to fetch `nrfxlib` (for NFC support).

To setup repository:

```
mkdir <SOME-PATH>/awf-zephyr-env
cd <SOME-PATH>/awf-zephyr-env
west init -m git@github.com:Sendrato/awf_zephyr.git -- mr main
west update
```

> NOTE: For full setup of CLion and Zephyr SDK, see `awareable-fw` repository and wiki.
