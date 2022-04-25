# ansible-role-git

Install and configure git client as well as clone git repos with ease.

## Requirements

N/A

## Role Variables

```yaml
users:
  - name: nobody
    fullname: "Nobody"
    home: /home/nobody
    email: nobody@gmail.com

git_ssh_private: "/root/.ssh/id_rsa"

force_git_clone: true

destination: "{{ users[0].home }}/Documents/Git"

github_repo_name:
  - stiliajohny/stiliajohny.github.io

gitlab_repo_name:
  - stiliajohny/stiliajohny.github.io
```

## Dependencies

N/A

## Example Playbook

```yaml
- hosts: servers
  roles:
    - { role: ansible-role-git }
```

## License

GPLv3

## Author Information

John Stilia - stilia.johny@gmail.com
