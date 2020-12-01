---
title: Play DTMF into a call
navigation_weight: 10
---

# Play DTMF into a call

This code snippet plays DTMF tones into the specified call.

## Example

Replace the following variables in the example code:

```snippet_variables
- UUID.VOICE
- DIGITS.VOICE
```

```code_snippets
source: '_examples/voice/play-dtmf-into-a-call'
application:
  type: voice
  use_existing: |
    Modifying an existing call requires that the <code>UUID</code> provided is a currently active call. To modify a call, you must use the same <code>VONAGE_APPLICATION_ID</code> and private key that were used to create the call.
```

## Try it out

When you run the code a series of DTMF tones is played
into the call identified with the specified UUID.
