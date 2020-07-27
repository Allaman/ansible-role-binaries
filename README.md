ansible-role-binaries
=========

Installs several applications via downloading the executable and placing it in Path on Linux based systems. Does **not** install the package via package manager. Additionally, install several Python packages via pip as user.

Installs via binary download:

- terraform
- awless
- aws
- broot
- docker
- helm
- githubcli
- stern
- popeye
- bat
- exa
- doctl
- kind
- kubectl
- k9s
- kops
- istioctl
- mdbook
- gh-md-toc
- fasd
- ripgrep
- xsv
- direnv
- entr
- nnn
- lf
- prettyping
- rofi
- delta
- yq
- jq

Install via pip:

- flake8
- testinfra
- molecule
- "molecule[docker]"
- yq
- ansible
- awscli
- thefuck
- neovim-remote
- httpie


Requirements
------------

Following programs must be in the path:

- unzip
- tar
- pip3
- gcc

For instance have a look at [ansible-role-basic](https://github.com/Allaman/ansible-role-basic)

Role Variables
--------------

See Example Playbook

Dependencies
------------

No dependencies

Example Playbook
----------------

```
---
- name: Playbook
  hosts: localhost
  connection: local
  pre_tasks:
    - set_fact:
        terraform_version: 0.12.24
        awless_version: 0.1.11
        helm_version: 3.1.1
        githubcli_version: 0.6.2
        stern_version: 1.11.0
        popeye_version: 0.7.1
        bat_version: 0.12.1
        exa_version : 0.9.0
        docker_version: 19.03.8
        docker_compose_version: 1.25.4
        doctl_version: 1.39.0
        ansible_ver: 2.9.6
        awscli_version: 1.18.2
        kind_version: 0.7.0
        kubectl_version: 1.18.0
        k9s_version: 0.19.1
        kops_version: 1.16.0
        istioctl_version: 1.5.1
        mdbook_version: 0.3.7
        fluxctl_version: 1.19.0
        kustomize_version: 3.5.5
        lazygit_version: 0.20.4
        kubeseal_version: 0.12.4
        argocdcli_version: 1.5.6
        xsv_version: 0.13.0
        ripgrep_version: 12.1.1
        fasd_version: 1.0.1
        direnv_version: 2.21.3
        entr_version: 4.6
        nnn_version: 3.3
        lf_version: r14
        rofi_version: 1.5.4
        delta_version: 0.3.0
        yq_version: 3.3.2
        jq_version: 1.6
  roles:
    - ansible-role-binaries
```

License
-------

MIT
