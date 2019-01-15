.PHONY: {{cookiecutter.name}}

init-{{cookiecutter.name}}: ;
	cd {{cookiecutter.name}} && vagrant up

cleanup-{{cookiecutter.name}}: ;
	cd {{cookiecutter.name}} && vagrant halt

deploy-{{cookiecutter.name}}:
	venv/bin/ansible-playbook {{cookiecutter.name}}/playbook.yml -i inventory.ini
