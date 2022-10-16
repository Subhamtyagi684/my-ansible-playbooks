# ansilble-playbooks

# playbook1.yaml
  1. It only creates a folder with a variable named provided using command
    ```
    ansible-playbook playbook1.yaml --extra-vars '{"folder_name":"theme_example"}'
    ```
  1. After creating folder it copies layout.j2 jinja template into layout.jade.

# playbook2.yaml
  1. It further extends the layout.jade and creates homepage.jade using layout.jade

# playbook3.yaml
  1. It asks src folder as a variable which is defined in a vars_file key .
  1. vars_file value is a value with a yaml file in which we can give scalar, dictionary and lists as variable which can further be handled by jinja templates with if-else and for loop.