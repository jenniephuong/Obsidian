>the owner of the resource decides who has access and has the power to change permissions for others e.g., OS, application level, an admin on a Linux server using chmod command
>
>![[Pasted image 20250415150035.png|500]]

various permission levels can be assigned 
- user based 
- job based
- project based 
- task based 

permissions are assigned to subjects

least restrictive due to individual complete control - can be weak as it relies on users correctly following the compliance rules when changing permissions, and attacks like trojan horses can change the permission level for attackers to take advantage of (data integrity)

owners can give higher permissions than needed 
permissions of users are inherited into other programs they execute, so that they can execute malware without knowing where the malware makes use of the users high privileges