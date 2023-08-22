# SeLinux Basic

- Security-Enhanced Linux (SELinux) is a Linux kernel security module that provides a mechanism for supporting access control security policies
 
- SELinux is implemented to provide an additional layer of protection, increase the control over processes execution, and protects against exploits by using multi level security.

- SELinux works by using `Labels` and `Type Enforcement`

	For example , “sshd” service executable configuration directory is labeled ssh_exec_t as seen below using the command utility ls -Z as shown below:
 
 ![image](https://github.com/Pavan-1997/SeLinux_Basic/assets/32020205/2cbd68ce-5ddc-448a-823d-2b2b8f993f84)

 Type Enforcement its the part where the policy dictates if for example within ssh process context running label ssh_exec_t to interact with a ssh file label
