# Linux
- netstat -aon
- ps -aef | grep { something }
- rm -r *
- ls -lrt
- kill -9 { pid }
- cp -r { from path } { to path }
- rm -r { File Directory }
- unzip { from zip folder } -d { to folder }
- mv { from directory } { to directory }
- find . -iname "*{file name}*"
- ifconfig | grep broadcase | awk '{print $2}'
- alias whatismyipaddress="echo $(ifconfig | grep broadcase | awk '{print $2}')"

# Gradle
- gradle build
- gradle clean build

# Maven
- mvn install
- mvn clean install
- mvn versions: set -N

# Nircmd
- nircmd execmd { ur command here }
- nircmd exec { ur bat file here }

# Node(npm) And Angular(ng)
- npm install
- npm prune
- npm ls
- ng serve

# GitHub
- git init
- git add .
- git remote add origin https://{ github repository }.git
- git commit -m "{ comment }"
- git push origin master --force
- git for-each-ref --sort=committerdate refs/heads/ --format='%(HEAD) %(color:yellow)%(refname:short)%(color:reset) - %(color:red)%(objectname:short)%(color:reset) - %(contents:subject) - %(authorname) (%(color:green)%(committerdate:relative)%(color:reset))'

# SVN
- svnserve -d -r { path to repository } --listen-host: 127.0.0.1 --listen-port: 3690
- svn info svn://localhost/$REPO_NAME

# Windows
- Xcopy { from path } { to path } /E /H /C /I
- sfc /scannow
- nslookup { domain name }
- tracert { domain name }
- ping { ip adress }

# Wildfly
- standalone.sh -b=0.0.0.0 -bmanagement=0.0.0.0

# sql
## sybase
select * from table_name
go
output to "C:/User/ping/outputfile.csv"

## sql server
BULK INSERT Sales.Orders
FROM 'C:/User/ping/outputfile.csv'
WITH ( FORMAT='CSV');

select t1.* from table1 t1
right outer join table2 t2
on t1.id = t2.id
