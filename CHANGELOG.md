## 0.2.1 (Unreleased)
## 0.2.0 (September 18, 2017)

DEPRECATED:

* `resource/triton_machine`: We've **un-deprecated** `networks` and now pass a list of network UUIDs for the machine to be attached to, `nic` is now used as a computed parameter rather than an input.

BUG FIXES:

* `resource/triton_machine`: Fix issues with machine network diffs ([#30](https://github.com/terraform-providers/terraform-provider-triton/issues/30))

## 0.1.3 (September 11, 2017)

BUG FIXES:

* `SDC_KEY_ID` may now be specified in either SHA256 or MD5 notation. ([#34](https://github.com/terraform-providers/terraform-provider-triton/issues/34))

## 0.1.2 (August 16, 2017)

FEATURES:

* `resource/triton_machine`: Locality hints can be specified to influence machine placement at machine create-time ([#31](https://github.com/terraform-providers/terraform-provider-triton/issues/31))
* `datasource/triton_image`: The `most_recent` argument can now be specified to disambiguate in the case of multiple images matching the specified criteria ([#23](https://github.com/terraform-providers/terraform-provider-triton/issues/23))
* `resource/triton_machine`: CNS tags can now be specified in a separate stanza ([#17](https://github.com/terraform-providers/terraform-provider-triton/issues/17))
* `resource/triton_machine`: User-defined metadata is now defined in a separate stanza ([#17](https://github.com/terraform-providers/terraform-provider-triton/issues/17))

## 0.1.1 (August 01, 2017)

FEATURES:

* *New Data Source:* `triton_image` ([#7](https://github.com/terraform-providers/terraform-provider-triton/issues/7))
* *New Data Source:* `triton_network` ([#13](https://github.com/terraform-providers/terraform-provider-triton/issues/13))

BUG FIXES:

* `resource/triton_machine`: Instances which fail during provisioning are now detected and tainted rather than timing out ([#10](https://github.com/terraform-providers/terraform-provider-triton/issues/10))
* `resource/triton_machine`: Metadata is now populated correctly ([#12](https://github.com/terraform-providers/terraform-provider-triton/issues/12))

## 0.1.0 (June 21, 2017)

NOTES:

* Same functionality as that of Terraform 0.9.8. Repacked as part of [Provider Splitout](https://www.hashicorp.com/blog/upcoming-provider-changes-in-terraform-0-10/)
