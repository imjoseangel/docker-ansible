[![Get your own image badge on microbadger.com](https://images.microbadger.com/badges/image/imjoseangel/docker-ansible.svg)](https://microbadger.com/images/imjoseangel/docker-ansible "Get your own image badge on microbadger.com")

## Ansible on Docker

A customized Docker Ansible image.

### Running

Run Ansible with a local playbook:

```shell
docker run -it --rm --name ansibleplay -v "$HOME/source":/source -w /source imjoseangel/docker-ansible ansible-playbook /source/myplaybook.yml 
```

or create a function:

```shell
ans() {
  docker run -it --rm --name ansibleplay -v "$HOME/source":/source -w /source imjoseangel/docker-ansible ansible-playbook "$1"
}
```

### License

Copyright © 2019 [imjoseangel](http://imjoseangel.github.com). Licensed under [the MIT license](https://github.com/imjoseangel/docker-tower/blob/master/LICENSE).
