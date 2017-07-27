# find-ami

Returns all the AMIs that matches the passed tags.

## Role Variables

Settable variables that are in defaults/main.yml.

* `base_ami.tags`: A list of all the tags that want to be searched.
* `base_ami.region`: The region in which the AMIs are.

## Example Playbook

It assumes you use the ec2 dynamic inventory

```yaml
- hosts        : localhost
  connection   : local
  gather_facts : no
  roles:
    - role: find-ami
```

## License

GPLv3

## Author

alexperez@paradigmadigital.com
