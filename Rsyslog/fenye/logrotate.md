# logrotate配置文将详解

### 参数
|参数|作用|
|--|--|
|daily|指定转储周期为每天|
|weekly|指定转储周期为每周|
|monthly|指定转储周期为每月|
|rotate 数字|指定日志文件删除之前转储的次数，0指没有备份，5指保留5个备份|
|compress|通过gzip压缩转储以后的日志|
|nocompress|不需要压缩时，用这个参数|
|create 权限 所有者 所属组|建立新的日志，同时指定新日志的权限与所有者和所属组|
|nocreate|不建立新的日志文件|
|errors address|存储时的错误信息发送到指定的Email地址|
|mail address|把转储的日志文件发送到指定的E-mail地址|
|notifempty|如果是空文件的话，则不进行日志轮替|
|missingok|如果日志不存在，则忽略该日志的警告信息|
|minsize 大小|日志轮替的最小值，也是日志到一定要达到这个最小值才会轮替，否则时间达到也不好轮替|
|size 大小|当日志文件大于指定大小才进行轮替，而不是按照时间轮替|
|dateext|使用日期作为日志轮替文件的后缀|
