This is possible to have top level playbook files import other playbook
files.  For example, a playbook called could include three
different playbooks, such as webservers, workers, dbservers, etc.

Running the site playbook would run all playbooks, while individual
playbooks could still be run directly.  This is somewhat like
the tag feature and can be used in conjunction for very fine grained
control over what you want to target when running ansible.


Note you can't use any variables in the include path here ( In nested path )
