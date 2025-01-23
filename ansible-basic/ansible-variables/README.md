## Here we have custom role directory created but in that there is no defination for main.yml so this script will not create role automatically, we have to create it by using galaxy

 $ansible-galaxy init /root/ansible-variables/roles/custom-role

 as this is for my version but as this command will create custom role for you then you can run the playbook to test variables without any role defination in task.

 to run the playbook

 $ansible-playbook --inventory /root/ansible-variables/inventory/ansible-variable-playbook/hosts /root/ansible-variables/ansible-variables-playbook.yml

 as just maintain the structure for the project same,if you want to change then you can but you have to mention correct path while running playbook.

## command to run while passing variable at runtime
 sudo ansible-playbook --inventory /root/ansible-variables/inventory/ansible-variable-playbook/hosts /root/ansible-variables/ansible-variables-playbook.yml --extra-vars '{"version":"1.0"}'


 sudo ansible-playbook --inventory /root/ansible-variables/inventory/ansible-variable-playbook/hosts /root/ansible-variables/ansible-variables-playbook.yml --extra-vars my-vars.yml

