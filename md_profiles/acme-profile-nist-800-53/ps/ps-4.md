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
  ps-04_odp.01:
    alt-identifier: ps-4_prm_1
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  ps-04_odp.02:
    alt-identifier: ps-4_prm_2
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
x-trestle-global:
  profile:
    title: NIST Special Publication 800-53 Revision 5 HIGH IMPACT BASELINE
  sort-id: ps-04
---

# ps-4 - \[Personnel Security\] Personnel Termination

## Control Statement

Upon termination of individual employment:

- \[a.\] Disable system access within {{ insert: param, ps-04_odp.01 }};

- \[b.\] Terminate or revoke any authenticators and credentials associated with the individual;

- \[c.\] Conduct exit interviews that include a discussion of {{ insert: param, ps-04_odp.02 }};

- \[d.\] Retrieve all security-related organizational system-related property; and

- \[e.\] Retain access to organizational information and systems formerly controlled by terminated individual.

## Control Assessment Objective

- \[PS-04a.\] upon termination of individual employment, system access is disabled within {{ insert: param, ps-04_odp.01 }};

- \[PS-04b.\] upon termination of individual employment, any authenticators and credentials are terminated or revoked;

- \[PS-04c.\] upon termination of individual employment, exit interviews that include a discussion of {{ insert: param, ps-04_odp.02 }} are conducted;

- \[PS-04d.\] upon termination of individual employment, all security-related organizational system-related property is retrieved;

- \[PS-04e.\] upon termination of individual employment, access to organizational information and systems formerly controlled by the terminated individual are retained.

## Control guidance

System property includes hardware authentication tokens, system administration technical manuals, keys, identification cards, and building passes. Exit interviews ensure that terminated individuals understand the security constraints imposed by being former employees and that proper accountability is achieved for system-related property. Security topics at exit interviews include reminding individuals of nondisclosure agreements and potential limitations on future employment. Exit interviews may not always be possible for some individuals, including in cases related to the unavailability of supervisors, illnesses, or job abandonment. Exit interviews are important for individuals with security clearances. The timely execution of termination actions is essential for individuals who have been terminated for cause. In certain situations, organizations consider disabling the system accounts of individuals who are being terminated prior to the individuals being notified.

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
