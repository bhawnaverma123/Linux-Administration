Experiment 4
Create the /home/consultants directory. Add write permission to the consultants group. Use the symbolic method for setting the appropriate permissions. Forbid others from accessing files in the /home/consultants directory. Use the octal method for setting the appropriate permissions. Change the default umask for the operator1 user. The new umask prohibits all access for users that are not in their group. Confirm that the umask is changed.

Experiment

Command to be used:

1.sudo mkdir -p /home/consultants

2.sudo chmod g+w /home/consultants

3.sudo chmod 770 /home/consultants

4.ls -ld /home/consultants

5.sudo mkdir -p /home/consultants

6.sudo groupadd consultants

7.sudo chown :consultants /home/consultants

8.sudo chmod g+w /home/consultants

9.sudo chmod 770 /home/consultants

10.sudo usermod -K UMASK=007 operator1

11.umask 007

12.umask

![image](https://github.com/user-attachments/assets/be81a4d3-bd7c-4f9e-91d9-03742389e64b)

![image](https://github.com/user-attachments/assets/7c155aa9-c7d9-4045-8bec-e1e38d440a98)

![image](https://github.com/user-attachments/assets/23ff2b63-7023-4ab6-8419-5644ff970736)


