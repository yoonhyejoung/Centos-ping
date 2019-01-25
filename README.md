# Centos-ping

Ping 명령어는 해당 서버가 현재 동작 중인지 아닌지 확인할 수 있는 가장 간단한 방법


ping명령어는 ICMP Protocol 명령어를 이용하고 이는 TCP/UDP 보다 하위인 Layer3에 위치


ping을 통해 2003년블랙스터웜이라는 DDOS 공격에 활용 


-proc 파일 시스템을 직접 수정 : Root 사용자가 조치


echo 1 > /proc/sys/net/ipv4/icmp_echo_ignore_all


echo 0 > /proc/sys/net/ipv4/icmp_echo_ignore_all


-sysctl 커맨드 사용하여 적용하는 방법 : Root 권한을 가진 사용자가 가능, sudo 명령어로 이용가능


Systcl-w net.ipv4.icmp_echo_ignore_all=1


Systcl-w net.ipv4.icmp_echo_ignore_all=0







Ping을 이용한 공격 ping of death, icmp redirect 공격 등이 있음


Proc : process의 약자 실행중인 프로세스의 정보와 cpu 메모리 등 시스템 정보가 있는 디렉토리
