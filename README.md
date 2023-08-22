# SeLinux Basic

- Security-Enhanced Linux (SELinux) is a Linux kernel security module that provides a mechanism for supporting access control security policies

 
- SELinux is implemented to provide an additional layer of protection, increase the control over processes execution, and protects against exploits by using multi level security.


- SELinux works by using `Labels` and `Type Enforcement`

  For example , “sshd” service executable configuration directory is labeled ssh_exec_t as seen below using the command utility ls -Z as shown below:
 
  ![image](https://github.com/Pavan-1997/SeLinux_Basic/assets/32020205/2cbd68ce-5ddc-448a-823d-2b2b8f993f84)

   Type Enforcement its the part where the policy dictates if for example within ssh process context running label ssh_exec_t to interact with a ssh file label


- There are two policies that can be used

   
		1. Targeted Policy : The default policy
		2. Minimum
		3. Multi-Level/Multi Category Security-(MLS) Policy: Can be enabled.
   


- SElinux has three modes of operation

	   
		1. Enforcing
		2. Disabled
		3. Permissive
  


- The modes of operation and the policy types are embedded inside “config” file which controls the state of the SELinux on the system.The file can be accessed using vim tool at
	```
	vi /etc/selinux/config
	```


- Check status of SE-Linux
	 
	  sestatus
	 	


- Change to SELinux Mode

  ```
  vi /etc/selinux/config
  ```
 
  ![image](https://github.com/Pavan-1997/SeLinux_Basic/assets/32020205/5ca76dce-2573-487f-a901-a6715720df11)
