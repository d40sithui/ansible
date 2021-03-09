# ansible
Ansible test scripts


1) Ansible is invoked using 
  ansible-playbook -e ENV=dev -i inventories/tcg tcg.yml
2) "dev" is the environment and also limits the playbook from running only on selected nodes under the [dev] parent under the inventories/tcg file. It also determines which var files will be imported as each environment I assume will have different variables. tcg.yml is the entry playbook which will eventually call /main/tasks.yml inside this role.
3) This playbook and role is not tested but conceptually I think it would work. It may requires some tweaks and possible syntax errors in some areas.
