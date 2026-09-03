# Change Log

This lists the new changes that have not yet been published in a normal release.

**In an attempt to avoid constant rebasing, please leave a blank line between
your addition and anything else already in this file.**

# Shared Improvements - Both Mk and Q

- tbd

- Enhancement: Support the unified opt-in signature hash. A PSBT can now ask for hash
  types 0x21, 0x22, 0x23, 0xa1, 0xa2 and 0xa3, and the resulting signature commits to
  every spent amount and scriptPubKey rather than only the one being signed, which
  removes CVE-2013-2292 and CVE-2020-14199 for the inputs that opt in. Because the
  message differs from every existing one, an opted-in transaction is also protected
  against replay onto any chain that does not implement the rule. Signing is unaffected
  unless a PSBT asks for it. Covers bare, P2SH and segwit v0 inputs; this tree does not
  sign taproot, so the rule's taproot script types are not reached.


# Mk Specific Changes

## 5.6.3 - 2026-09-xx

- tbd


# Q Specific Changes

## 1.5.3Q - 2026-09-xx

- tbd


