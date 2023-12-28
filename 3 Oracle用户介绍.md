## 三、Oracle用户介绍

### 相关链接：[05Oracle用户介绍_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1Eq4y127K2/?p=5&spm_id_from=pageDriver&vd_source=e6711227b0ce09c2866b8d609bbe7b46)

最主要的三个内置的系统用户（最大的区别就是权限不同）

1. sys用户

   sys是Oracle中的超级账户，拥有的权限最大。可以完成数据库的所有管理任务。

2. system用户

   没有sys权限大，通常用来创建一些用户查看管理信息的表或视图。不建议使用smsystem来创建一些与管理无关的表或者视图。

3. scott用户

   scott:是oracle提供的示例用户，提供了一些学习oracle操作的数据表。如：emp、dept、salgrade、bonus表，表里有一些基础数据

★sys和system在登录时的区别

sys和system在登录Oracle时，sys只能以系统管理员(sysdba)或系统操作员(sysoper)的权限登录，即登录时要给定角色（用as给定），而system可以直接登录(normal)。



ps：可以在sqlplus登录后输入  select * from all_users;  来在  数据字典表all_users  里面看全部系统用户