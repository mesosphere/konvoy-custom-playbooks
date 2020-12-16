This playbook re-registers SLES instances with update servers in order to resolve this issue: <https://www.suse.com/support/kb/doc/?id=000019085>. 

> SUSE software repositories are not configured for a SLE Pay-As-You-Go cloud instance. 
> Because of this, zypper or YaST cannot be used to install new software or migrate to a new service pack.

Konvoy may encounter this issue as a failure to install packages.
To resolve it, run `konvoy run playbook playbook.yaml` and then resume the deployment with `konvoy up`.
