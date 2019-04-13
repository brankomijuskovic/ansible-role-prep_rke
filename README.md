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
+ [RKE supported](https://rancher.com/docs/rke/v0.1.x/en/installation/os/) versions aren't found in the [Docker repository](https://download.docker.com/linux/ubuntu/dists/bionic/) for Ubuntu bionic at this time, the install will fail unless using something unsupported such as "18.03.1\~ce~3-0\~ubuntu"
