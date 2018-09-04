#python_ldap
#authentication from windows AD
#python version:2.7
#windows version: windows server 2008 R2 
#os: Centos7 1805
#author: jbqh
#lastupdate: 2018-09-04 22:10:00

#need python-ldap package
#yum install python-ldap

#example:
ldapServer = 'ldap://127.0.0.1:389'
baseDN = 'dc=test,dc=com'
bindDN = 'cn=user1,ou=myou,dc=test.dc=com'
bindPassword = 'userpassword'
searchFilter = '(sAMAccountName=%s)'
ldap.set_option(ldap.OPT_REFERRALS,0)
