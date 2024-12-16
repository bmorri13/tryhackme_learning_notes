# Advent of Cyber 2024

## Active Directory - LDAP

- Went over AD sturcures, what makes up AD such as users, groups, domains, OU's, forests, etc.
- Example Domain structure - Domains: Logical groupings of network resources such as users, computers, and services. They serve as the main boundary for AD administration and can be identified by their Domain Component and Domain Controller name. Everything inside a domain is subject to the same security policies and permissions. - Organisational Units (OUs): OUs are containers within a domain that help group objects based on departments, locations or functions for easier management. Administrators can apply Group Policy settings to specific OUs, allowing more granular control of security settings or access permissions. - Forest: A collection of one or more domains that share a standard schema, configuration, and global catalogue. The forest is the top-level container in AD. - Trust Relationships: Domains within a forest (and across forests) can establish trust relationships that allow users in one domain to access resources in another, subject to permission.
  > Example:

```bash
DN=CN=Mayor Malware, OU=Management, DC=wareville, DC=thm
```

### Room Example

- For the lab we ran through using event viewer to view AD logs, search for key items for the flags and then used GPO list commandlets to get the information we required.
