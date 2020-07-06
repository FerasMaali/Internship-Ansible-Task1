# Internship-Ansible-Task1

## For copying file:
```
ansible-playbook \
        -i hosts \
        --extra-vars "destination_dir=/absolute/path/to/destination/directory \
        [suffix=_some_suffix]" \
        [input_file=path/to/input/file] \
        copy_playbook.yml
```

## For doing diff:
```
ansible-playbook \
        -i hosts \
        --extra-vars "first_run=/first/run/destination \
        second_run=/second/run/destination" \
        diff_playbook.yml
```

## Note
The given paths must always be absolute paths (except input_file)
