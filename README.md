This is a simple library to check if a string is a reserved keyword in sql. It currently supports keywords from  postgresql_10, 
postgresql_8.1, sql_2003, sql_1999, sql_92.  Defaults to postgresql_10

usage

import issql

issql.is_reserved('ALL')
>> True

issql.is_reserved('YES') 
>> False


issql.is_reserved('ABS') 
>>False


issql.is_reserved('ABS', version='sql_2003') 
>>True
