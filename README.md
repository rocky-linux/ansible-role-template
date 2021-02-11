CI Badge

# Ansible template role
Role that fulfills $x need and there was not some sort of equivalent elsewhere.

## Getting started
Ensure all dependencies are installed/met and then do the following:
1. Get the development repository: `git clone repo`
2. Install pre-commit: `pre-commit install`
3. Make edits as required as well as following the customization section
4. Run `pre-commit` to ensure we're good
5. Do your necessary development work for this role
6. Run `pre-commit` again to ensure you're good to go.
7. Optional: `molecule converge`

## Dependencies
This repo expects 3 things installed on your local machine:
1. [pre-commit](https://pre-commit.com/)
2. [ansible-lint](https://github.com/ansible-community/ansible-lint)
3. [yamllint](https://github.com/adrienverge/yamllint)

### Customization
Note that this is optional and not a full requirement for your role.

1. [molecule/requirements.yml](molecule/requirements.yml) - Update with any required roles or collections that you may be leveraging for your role.
2. [molecule/default/converge.yml](molecule/default/converge.yml) - Update with your role name
3. [molecule/default/molecule.yml](molecule/default/molecule.yml) - Update with desired distributions and extra playbooks if necessary
4. [github](github) - Rename this to `.github` and then `git push`, this will set up yamllint, ansible-lint and a CI check job for the `main` branch
   1. Note that if you are using a SAML token, this may fail. You can created the files within the Github web app.

### Optional
The github actions are configured to run the molecule tests automatically, but if you want to load them locally, you will need to install molecule to your machine.

## Changelog
The [changelog](./CHANGELOG.md) is stored externally

