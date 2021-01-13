## Description

<!-- Please write a short summary for this change. If it's a playbook, explain what it does. -->

## Best Practices checklist
<!---  Put an `x` in all the boxes that apply: -->

### General
- [ ] Go over texts with @stackpulse/product
- [ ] Explicitly discuss the _playbook name_, _image_ and _badges_
- [ ] Explicitly consider various _benefits_. As a rule of thumb, there should be 2-3 of them

### New playbooks
- [ ] Tested Playbook in a production tenant
- [ ] Added a link in the [README.MD](https://github.com/stackpulse/playbooks/blob/master/README.md)

### Playbook structure
- [ ] For improved human-readability, please add a new empty line between the steps
- [ ] Please add a one-liner comment block before each step, for example: `# Retrieve long connections from the database server`
- [ ] When considering step IDs, please use short, but descriptive terms, explaining what is being done, such as `retrieve_connections_data` or `update_storage_size`
- [ ] When writing params descriptions, start with a capital letter and phrase as a short sentence, such as `User name for database connection` or `Address of the database cluster`


## Screenshot

<!-- please include a screenshot or a GIF/MP4 of how it works. Validate the screenshot with @stackpulse/product as well: make sure that it provides a good example for the value of the playbook and has high chances of causing a reaction of "Yes, I understand how it can help me" from a person looking at it.  -->
