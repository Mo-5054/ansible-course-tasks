## Ansible Inventory File Hint

If you want to use the following inventory file:
[database] db1 ansible_host=18.204.205.131 ansible_ssh_user=ec2-user ansible_ssh_private_key_file=/home/mohamed/momo.pem db2 ansible_host=18.206.250.159 ansible_ssh_user=ec2-user ansible_ssh_private_key_file=/home/mohamed/momo.pem

Make sure to update the following values before using it:
- `ansible_host` → Replace with your actual server IP for `db1` and `db2`.
- `ansible_ssh_user` → Use the correct SSH username for your environment.
- `ansible_ssh_private_key_file` → Set the correct path to your private key file.

🔹 **Example (Updated Configuration):**

[database] 
db1 ansible_host=<your-db1-ip> ansible_ssh_user=<your-ssh-user> ansible_ssh_private_key_file=<your-private-key-path> db2 ansible_host=<your-db2-ip> ansible_ssh_user=<your-ssh-user> ansible_ssh_private_key_file=<your-private-key-path>
