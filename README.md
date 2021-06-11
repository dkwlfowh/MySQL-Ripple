# MySQL-Ripple
1. Ripple 서버는 Replication과 같은 방식으로 MySQL Master에 연결하지만 MySQL에서 데이터 사본을 생성하는 대신 Ripple은 binlog를 다운로드하여 로컬에 저장한다.그런 다음 MySQL 서버를 마스터 대신 Ripple에서 복제하도록 지정할 수 있습니다. Ripple은 다운로드 한 binlog를 마스터와 동일한 방식으로 제공합니다. 이렇게하면 MySQL 마스터의로드를 크게 줄이고 binlog의 내구성을 향상시킬 수 있습니다.

2. Ripple은 GTID (각각 MariaDB 및 MySQL 버전)를 사용하여 MariaDB 및 MySQL과의 복제를 지원합니다. 파일 이름 및 위치를 사용한 복제는 지원되지 않습니다. Ripple은 MariaDB 10.0 및 MySQL 5.6 및 5.7에서 테스트되었지만 이후 버전에서도 작동 할 것입니다.

https://github.com/dkwlfowh/MySQL-Ripple/issues/1#issue-918673901
