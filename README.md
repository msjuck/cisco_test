# [중부]DNSN-ACSM-IMS-L3SW-2 CONSISTENCY LOG해소를 위한 SUP 절체 작업


작성자	문영민	작업자		승인자	최홍준M
Version	1.1	시스템	DNSN-ACSM-IMS-L3SW-1, 2	작성일	2017/09/27
작업개요	[중부]DNSN-ACSM-IMS-L3SW-2 CONSISTENCY LOG해소를 위한 SUP 절체 작업
작업목적	FM-6-FM_CONSISTENCY_CHECK_LOG_STATUS: Consistency Checker found inconsistency 에러 지속 발생(서비스영향X)
작업일자	2017-10-11 02:00 ~ 2017-10-11 05:00

구분	세부 내용
요청 부서	IP NOC
목적	FM-6-FM_CONSISTENCY_CHECK_LOG_STATUS: Consistency Checker found inconsistency 에러 지속 발생(서비스영향X)
작업 내용	■ 제목 : DNSN-ACSM-IMS-L3SW-2 CONSISTENCY LOG해소를 위한 SUP 절체 작업
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
