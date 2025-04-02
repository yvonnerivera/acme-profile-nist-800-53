---
x-trestle-set-params:
    # This section contains the parameters that are part of this control.
  # Each parameter has properties. Only the profile-values and display-name properties are editable.
  # The other properties are informational.
  #
  # The values property for a parameter represents values inherited from the OSCAL catalog.
  # To override the catalog settings, use bullets under profile-values as shown below:
  #
  #   profile-values:
  #     - value 1
  #     - value 2
  #
  # If the "- <REPLACE_ME>" placeholder appears under profile-values, it is the same as if
  # the profile-values property were left empty.
  #
  # Some parameters may show an aggregates property which lists other parameters. This means
  # the parameter value is made up of the values from the other parameters. For parameters
  # that aggregate, profile-values is not applicable.
  #
  # Property param-value-origin is meant for putting the origin from where that parameter comes from.
  # In order to be changed in the current profile, profile-param-value-origin property will be displayed with
  # the placeholder "<REPLACE_ME>" for you to be replaced. If a parameter already has a param-value-origin
  # coming from an inherited profile, do no change this value, instead use profile-param-value-origin as follows:
  #
  #    param-value-origin: DO NOT REPLACE - this is the original value
  #    profile-param-value-origin: <REPLACE_ME> - replace the new value required HERE
  #
  si-7_prm_1:
    aggregates:
      - si-07_odp.01
      - si-07_odp.02
      - si-07_odp.03
    profile-param-value-origin: <REPLACE_ME>
  si-7_prm_2:
    aggregates:
      - si-07_odp.04
      - si-07_odp.05
      - si-07_odp.06
    profile-param-value-origin: <REPLACE_ME>
  si-07_odp.01:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07_odp.02:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07_odp.03:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07_odp.04:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07_odp.05:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07_odp.06:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
x-trestle-global:
  profile:
    title: NIST Special Publication 800-53 Revision 5 HIGH IMPACT BASELINE
  sort-id: si-07
---

# si-7 - \[System and Information Integrity\] Software, Firmware, and Information Integrity

## Control Statement

- \[a.\] Employ integrity verification tools to detect unauthorized changes to the following software, firmware, and information: {{ insert: param, si-7_prm_1 }} ; and

- \[b.\] Take the following actions when unauthorized changes to the software, firmware, and information are detected: {{ insert: param, si-7_prm_2 }}.

## Control Assessment Objective

- \[SI-07a.\]

  - \[SI-07a.[01]\] integrity verification tools are employed to detect unauthorized changes to {{ insert: param, si-07_odp.01 }};
  - \[SI-07a.[02]\] integrity verification tools are employed to detect unauthorized changes to {{ insert: param, si-07_odp.02 }};
  - \[SI-07a.[03]\] integrity verification tools are employed to detect unauthorized changes to {{ insert: param, si-07_odp.03 }};

- \[SI-07b.\]

  - \[SI-07b.[01]\] {{ insert: param, si-07_odp.04 }} are taken when unauthorized changes to the software, are detected;
  - \[SI-07b.[02]\] {{ insert: param, si-07_odp.05 }} are taken when unauthorized changes to the firmware are detected;
  - \[SI-07b.[03]\] {{ insert: param, si-07_odp.06 }} are taken when unauthorized changes to the information are detected.

## Control guidance

Unauthorized changes to software, firmware, and information can occur due to errors or malicious activity. Software includes operating systems (with key internal components, such as kernels or drivers), middleware, and applications. Firmware interfaces include Unified Extensible Firmware Interface (UEFI) and Basic Input/Output System (BIOS). Information includes personally identifiable information and metadata that contains security and privacy attributes associated with information. Integrity-checking mechanisms—including parity checks, cyclical redundancy checks, cryptographic hashes, and associated tools—can automatically monitor the integrity of systems and hosted applications.

# Editable Content

<!-- Make additions and edits below -->
<!-- The above represents the contents of the control as received by the profile, prior to additions. -->
<!-- If the profile makes additions to the control, they will appear below. -->
<!-- The above markdown may not be edited but you may edit the content below, and/or introduce new additions to be made by the profile. -->
<!-- If there is a yaml header at the top, parameter values may be edited. Use --set-parameters to incorporate the changes during assembly. -->
<!-- The content here will then replace what is in the profile for this control, after running profile-assemble. -->
<!-- The current profile has no added parts for this control, but you may add new ones here. -->
<!-- Each addition must have a heading either of the form ## Control my_addition_name -->
<!-- or ## Part a. (where the a. refers to one of the control statement labels.) -->
<!-- "## Control" parts are new parts added after the statement part. -->
<!-- "## Part" parts are new parts added into the top-level statement part with that label. -->
<!-- Subparts may be added with nested hash levels of the form ### My Subpart Name -->
<!-- underneath the parent ## Control or ## Part being added -->
<!-- See https://oscal-compass.github.io/compliance-trestle/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring for guidance. -->
