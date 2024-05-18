#book 

**P**luggable **A**uthentication **M**odules provode a centralised module for authentication, it is pluggable because there are different [[PAM]]s for different authentication sources. It mains advantages are:
- provide prevalent pattern for authentication for wide variety of applications
- It is flexible, and gives a lot of control to administrators

## Configuration
Each application that uses [[PAM]] have it's file in `/etc/pam.d/`. For example [[sudo]] have it's configuration in `/etc/pam.d/sudo`. Configuration is written in simple language:
- `session    required   pam_limits.so` means:
  - `session` Change or manage a user session
  - `required` It will be successful only if this module is successful
  - `pam_limits.so` It is name of a module, This one specifies limits on resources
  In summary it will enforce that, whenever user runs [[sudo]], the limits written in system configuration will be applied.
- `auth    sufficient    pam_permit.so` means:
  - `auth` Change something in authentication method
  - `sufficient` If this module success, that is enough to authenticate.
  - `pam_permit.so` This module always success.
  In summary it will let everyone run a [[sudo]] command without need to know password.
- `auth    sufficient   pam_rootok.so` means:
  - `pam_rootok.so` This module check whether you are a root or not.
  It will not ask you for password when you are already root.