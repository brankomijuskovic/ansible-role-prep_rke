# Ansible Role



## Purpose
  Prepare server for Rancher Kubernetes Engine (rke).
  
----

## Execution
<pre>
    - hosts: all
      user: root
      tasks:
      - include_role:
          name: ansible-role-prep_rke

</pre>

----

## Notes
+ Debian based servers with Apt type package management ONLY
