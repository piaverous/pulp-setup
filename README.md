# Setting up a Pulp instance

## Local setup

- Install ansible 2.12 or higher
- Install dependencies
    - `ansible-galaxy install -r requirements.txt`
- Setup your `hosts.yml` file
    - Set the right host for your target machine

## Running it

- Install Pulp
    - `ansible-playbook -i hosts.yml plays/install.yml`
- Setup a simple repository and sync it with its remote
    - `ansible-playbook -i hosts.yml plays/repos.yml`

