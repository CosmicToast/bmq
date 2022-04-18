# Bunker/Bash MQ
Does not actually need bash, will work with POSIX sh.
Requires nmap's ncat and base64.

Read the bunker labs [post](https://pencil.toast.cafe/bunker-labs/a-message-queue-in-shell) for more context.

## Gotchas

### Base64 Wrapping
`base64` is non-standard, and some implementations do row wrapping.
In case yours does, change the invocations to not wrap (usually, `-w 0`).
