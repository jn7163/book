##MySQL安装、卸载

Ubuntu下
	
	sudo apt-get install mysql-server//安装
	sudo apt-get autoremove mysql-server//卸载

##MySQL管理
	
MacOS
	
	sudo /Library/StartupItems/MySQLCOM/MySQLCOM start//启动
	sudo /Library/StartupItems/MySQLCOM/MySQLCOM stop//停止
	sudo /Library/StartupItems/MySQLCOM/MySQLCOM restart//重启

Ubuntu
	
	//init.d方式
	sudo /etc/init.d/mysql start//启动
	sudo /etc/init.d/mysql stop//停止
	sudo /etc/init.d/mysql restart//重启
	//startup方式
	sudo start mysql//启动
	sudo stop mysql//停止
	sudo restart mysql//重启
	//service方式
	sudo service mysql start//启动
	sudo service mysql stop//停止
	sudo service mysql restart//重启

MySQL操作
	
	mysql -u root -p//登录MySQL,提示输入Password
	status;//查看服务器状态
	show databases;//查询数据库列表
	use `dbname`;//选择数据库
	show tables;//查看数据库下的所有表
	//查询表结构
	describe table;
	desc table;
	show columns from table;
