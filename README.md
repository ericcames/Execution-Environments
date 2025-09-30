# Execution-Environments

**Red Hat Ecosystem Catalog**
Red Hat Base Images for use in building Execution/Descision Environments.

[Container results for ansible-automation-platform](https://catalog.redhat.com/en/search?searchType=Containers&q=ansible-automation-platform&p=1 "Container results for ansible-automation-platform")<br>

**Execution environment definition**
[Execution environment definition](https://ansible.readthedocs.io/projects/builder/en/stable/definition/#overview "Execution environment definition")<br>

**Manual container build process**
```
1. Create your execution-environment.yml
2. ansible-builder build -v3 -t cohesity_rhel9:1.0.0
3. podman images
   a. localhost/cohesity_rhel9
4. podman tag localhost/cohesity_rhel9:1.0.0 quay.io/zigfreed/cohesity_rhel9:1.0.0
5. podman login quay.io
6. podman push quay.io/zigfreed/cohesity_rhel9:1.0.0
7. Is the container public?
8. Move the latest tag
```
