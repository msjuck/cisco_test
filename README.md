# [중부]DNSN-ACSM-IMS-L3SW-2 CONSISTENCY LOG해소를 위한 SUP 절체 작업

-------------
```
1. 작성자	: 문영민	
2. 작업자	: 문영민
3. 승인자	: 최홍준M
3. Version	: 1.1	
4. 시스템	: DNSN-ACSM-IMS-L3SW-1, 2	
5. 작성일	: 2017/09/27
6. 작업개요	: [중부]DNSN-ACSM-IMS-L3SW-2 CONSISTENCY LOG해소를 위한 SUP 절체 작업
7. 작업목적	: FM-6-FM_CONSISTENCY_CHECK_LOG_STATUS: Consistency Checker
             found inconsistency 에러 지속 발생(서비스영향X)
8. 작업일자	: 2017-10-11 02:00 ~ 2017-10-11 05:00
```
-------------
구분	세부 내용
-------------
```
1. 요청 부서	: IP NOC
2. 목적	: FM-6-FM_CONSISTENCY_CHECK_LOG_STATUS: Consistency Checker found inconsistency 에러 지속 발생(서비스영향X)
3. 작업 내용	: 
■ 제목 : DNSN-ACSM-IMS-L3SW-2 CONSISTENCY LOG해소를 위한 SUP 절체 작업
■ 배경 :FM-6-FM_CONSISTENCY_CHECK_LOG_STATUS: Consistency Checker found inconsistency 에러 지속 발생(서비스영향X)
■ 대상시스템 :DNSN-ACSM-IMS-L3SW-2
■ 고장시 영향받는 시스템/서비스 : IMS
■ 서비스 중단 최소화 방안 : 1호기로 절체
■ 작업 상세 내용 :
1. 중부NOC 서비스 상태확인
2. DNSN-ACSM-IMS-L3SW-2 설정확인
3. DNSN-ACSM-IMS-L3SW-2 SUP절체 ( Main -> Backup )
4. Log 미발생확인 및 SUP원복 ( Backup -> Main)
5. 중부NOC와 서비스 상태(HDV) 확인하면서 작업 진행할 것
원복작계도 작성해주세요!
작업 대상
시스템	DNSN-ACSM-IMS-L3SW-1, 2
서비스 영향도	-IMS
서비스 연동
장비	- 
요청 사항	-
```


<pre><code>
[둔산] DNSN-ACSM-IMS-L3SW-1
* 해당 작업 후 서비스 이상 유무 확인 
conf t
!
interface Vlan32
 standby 32 priority 115
 standby 32 preempt
!(HSRP 절체 후 preempt 삭제)
 no standby 32 preempt
!
interface Vlan82
 standby 82 priority 115
 standby 82 preempt
!(HSRP 절체 후 preempt 삭제)
 no standby 82 preempt
!
end
!
wr
</code></pre>
