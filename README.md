###############################
# Author: Boni Yeamin        #
# Date:                      #
# This is Ansible LAMP Stack Project       #
# Version : v1               #
###############################

# Ansible LAMP Stack

This Ansible project automates the setup of a LAMP (Linux, Apache, MySQL, PHP) stack on multiple servers. It provides a structured approach to configure and manage the LAMP stack, making it easy to deploy and maintain web applications.

## Project Structure

The project structure is organized as follows:

- `inventories/`: Contains inventory files for different environments.
- `playbooks/`: Holds Ansible playbooks for configuring the LAMP stack.
- `roles/`: Contains reusable Ansible roles for Apache, MySQL, and PHP configuration.
- `ansible.cfg`: Ansible configuration file to specify defaults.

## Usage

1. **Populate Inventory**:
   - Update the inventory files (`inventories/production/hosts`) with the IP addresses of your servers.

2. **Set Variables**:
   - Customize variables in `inventories/production/group_vars/all.yml` according to your requirements.

3. **Ensure SSH Key Access**:
   - Make sure your SSH key specified in `ansible.cfg` has access to all servers without needing a password.

4. **Run the Playbook**:
   - Execute the playbook to configure the LAMP stack:
     ```bash
     ansible-playbook playbooks/lamp-stack.yml
     ```

5. **Verify Configuration**:
   - After execution, verify that the LAMP stack is correctly configured on each server.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or create a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
