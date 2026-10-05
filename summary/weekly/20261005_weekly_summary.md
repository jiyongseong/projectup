# Azure 주간 업데이트 요약 - 2026년 10월 05일

## 🗃️ 데이터베이스 및 하이브리드 클라우드

지난주 Azure에서는 데이터베이스 및 하이브리드 클라우드 영역에서 대규모 혁신이 진행되었습니다. Azure SQL Database, Azure SQL Managed Instance, Azure Database for PostgreSQL 등 주요 플랫폼은 확장성과 성능을 대폭 개선하며, 비용 효율적 운영과 AI·검색 시나리오를 위한 기능들이 정식 지원 혹은 미리 보기(Preview)로 출시되었습니다. 고객 관리 키(CMK)를 테넌트 간 분리해 저장하는 기능은 SaaS, ISV 등 보안과 컴플라이언스 요구가 높은 고객에게 실질적 편익을 제공합니다. 또한 자동 인덱스 압축, 브라우저 기반 쿼리 에디터, 벡터 검색 등은 데이터 관리와 분석의 효율을 극대화하며, SQL DevOps와 마이그레이션 자동화 기능은 개발·운영 현장에서 생산성을 대폭 개선합니다. Azure Arc와 Microsoft Fabric 통합, Grafana 연동으로 통합 모니터링 및 관리 경험 역시 한층 진화하였습니다. 이들 변화는 데이터 기반 비즈니스 환경의 혁신적 전환을 뒷받침합니다.

### [Azure SQL Database의 벡터 검색 및 벡터 인덱스 정식 지원](https://azure.microsoft.com/updates?id=571800)
DiskANN 기반 벡터 인덱스와 T-SQL 벡터 검색 기능이 정식 지원되어, AI 검색·RAG·추천·이미지 검색 등 대규모 데이터에서 관계형 쿼리와 유사도 검색을 결합할 수 있습니다.

### [Azure Database for PostgreSQL Flexible Server의 크로스 테넌트 CMK 지원](https://azure.microsoft.com/updates?id=571783)
암호화 키를 별도 Microsoft Entra 테넌트의 Key Vault/HSM에 저장하여 데이터 운영과 키 관리 분리를 실현, SaaS·ISV의 보안·컴플라이언스 요건 충족을 지원합니다.

### [Azure SQL late-September 2026 업데이트](https://azure.microsoft.com/updates?id=571643)
Hyperscale Premium 시리즈에 160/192-vCore 추가, 자동 인덱스 압축, 브라우저 기반 쿼리 에디터 등 대형 데이터 워크로드 및 개발 환경 확장성을 크게 강화했습니다.


## 🖥️ 컴퓨트 및 가상 머신

컴퓨트와 가상 머신 분야에선 신제품 라인업과 자동화 기능 미리 보기, 운영체제 지원 확대가 두드러졌습니다. 5세대 AMD EPYC 기반 Lasv5, Laosv5 시리즈는 NVMe 대용량 스토리지와 200Gbps 네트워크, 최대 160 vCPU 등 고성능 분산 워크로드에 최적화된 사양을 제공하며, Azure Boost SSD 등 최신 기술로 성능과 보안을 보장합니다. VM Scale Set의 자동 영역 배치 미리 보기(Preview)는 멀티 리전 환경에서 관리 편의성을 높이고 장애 복원력·성능 확장성을 개선합니다. SQL Server on VM 성능 모니터링 미리 보기, Ubuntu 26.04 지원 등도 운영 효율과 현장 적용성을 크게 향상시키고 있습니다. VM 및 OS의 지원 종료 정책 강화와 함께 현대화 마이그레이션 가이드가 제공되어, 미래 인프라 전환도 원활히 준비할 수 있습니다.

### [Lasv5 및 Laosv5 스토리지 최적화 VM 시리즈 정식 지원](https://azure.microsoft.com/updates?id=572630)
최신 AMD 기반 대용량·고성능 VM라인업으로 대규모 분산 워크로드·AI/HPC 환경에 최적화, 스토리지와 네트워크 혁신을 실현합니다.

### [VM Scale Set 자동 영역 배치 미리 보기](https://azure.microsoft.com/updates?id=571075)
자동 배치 기능은 멀티 리전·멀티존 환경에서 VM 인스턴스 분산 정책을 자동화해 확장성, 장애 복원력을 극대화합니다.

### [Azure Virtual Machines의 SQL 서버 성능 모니터링 미리 보기](https://azure.microsoft.com/updates?id=571894)
SQL IaaS 에이전트 기반 성능 데이터 수집·분석, Azure Data Explorer 및 Fabric 연동 대시보드로 운영·성능관리 효율이 대폭 향상되었습니다.


## 💾 스토리지 및 Azure NetApp Files

스토리지와 파일 서비스 영역에서 Azure NetApp Files를 중심으로 고성능·대용량 지원이 확대되었습니다. 프리미엄/울트라 서비스에서 쿨 액세스 QoS와 핫/쿨 자동 최적화가 도입되어 HPC, EDA 등 고성능 환경에서 비용·성능을 효율적으로 조절할 수 있습니다. 대용량 볼륨 breakthrough mode는 최대 2PiB, 80GiBps, 볼륨당 6개 엔드포인트로 설계되어, 초저지연·대규모 데이터 워크로드에 대응 가능합니다. Microsoft Entra Kerberos 인증 지원(Preview)은 하이브리드·클라우드 SMB 인증 아키텍처를 단순화하고, AD 의존성을 제거합니다. 룩셈부르크 리전 Extended Zone 론칭으로 데이터 레지던시 및 저지연 서비스 적용범위가 확장되었습니다.

### [Azure NetApp Files: 대용량 볼륨 breakthrough mode 정식 지원](https://azure.microsoft.com/updates?id=573027)
최대 2PiB 스토리지, 80GiBps 성능, 볼륨당 6개 엔드포인트로 HPC·EDA·대규모 워크로드에 맞춤형 설계 제공.

### [Azure NetApp Files: 프리미엄/울트라 서비스 쿨 액세스 QoS 개선](https://azure.microsoft.com/updates?id=573032)
핫/쿨 저장소간 동적 처리와 자동화된 성능·비용 최적화가 적용되어 데이터 처리 효율이 극대화됩니다.

### [Azure NetApp Files: Microsoft Entra Kerberos 인증 미리 보기](https://azure.microsoft.com/updates?id=573041)
SMB 볼륨에서 엔트라ID 기반 클라우드/하이브리드 인증 지원, AD 의존성 제거 및 인증 아키텍처 현대화 실현.


## 🧑‍💼 관리 & 거버넌스 · 개발도구 · Copilot

관리 및 거버넌스, 개발 생산성 강화 영역에서 GitHub Copilot과 연계된 Azure 캔버스, SSMS DevOps, SQL Formatter 등이 발표되었습니다. Azure canvases는 Copilot 대화와 리소스·워크플로우·대시보드를 통합, 개발과 운영의 실시간 관리를 지원합니다. SSMS의 SQL 프로젝트 기반 DevOps는 CI/CD 연동과 자동화로 데이터베이스 운영 효율을 극대화하며, Visual Studio Code용 SQL Formatter의 정식 지원은 쿼리 표준화와 생산성 향상을 제공합니다. SQL Migration Agent Skills 등 AI 기반 마이그레이션 자동화, Azure SQL Dev Hub 등 포괄적 개발 허브도 론칭되며, Fabric 연동 대시보드와 통합 모니터링 역시 강화되었습니다. 이밖에도 신규 SDK, 데이터 거버넌스 도구의 지속적 개선과 Copilot 인공지능 기반 개발 환경 도입으로 Azure 소프트웨어 혁신이 가속화되고 있습니다.

### [Azure canvases for GitHub Copilot 발표](https://azure.microsoft.com/updates?id=573385)
Copilot 대화와 Azure 리소스·대시보드·워크플로우 통합 workspace로, 실시간 개발·운영 관리와 AI 기반 협업이 한곳에서 가능합니다.

### [SSMS 기반 데이터베이스 DevOps 지원](https://azure.microsoft.com/updates?id=571852)
SQL database project 연동·자동화로 테이블·SP 등 관리, CI/CD 연동 지속적 개발환경 제공, DevOps 생산성 향상 실현합니다.

### [Visual Studio Code용 SQL Formatter 정식 지원](https://azure.microsoft.com/updates?id=571872)
코드 스타일 맞춤 SQL 포맷터 도입으로 개발 쿼리 표준화, 수동 포맷 없이 생산성 및 코드 품질이 대폭 상승합니다.

 
## 📅 서비스 퇴출 및 지원 종료 안내

지난주 Azure에서는 여러 VM 시리즈와 서비스의 지원 종료(retirement)가 발표되었습니다. Arc-SCVMM, Functions v1 on Container Apps, IoT Central, HPC Pack 등은 수년 내 공식 지원이 종료될 예정이며, 각 서비스별 마이그레이션 경로와 가이드가 함께 공개되고 있습니다. 특히 VM 시리즈(Dcsv3, Dv3/Ev3/Esv3/NVv3/NVv4 등)는 순차적으로 사용 중단 및 퇴출 정책을 따라야 하며, 미리 현대화 및 업그레이드 플랜을 준비해야 서비스 연속성이 보장됩니다. Azure IoT Central 고객은 IoT Hub, DPS, Microsoft Fabric 등으로의 전환을 위한 playbook 및 파트너 지원이 제공되고, Arc-SCVMM 사용자는 Arc-enabled Servers 등 대안 솔루션으로의 마이그레이션 안내를 받아야 합니다. 커뮤니티 Q&A, Azure 공식 지원 채널도 함께 활성화되어 대규모 인프라 변경을 대비할 수 있습니다.

### [Azure Arc-SCVMM 지원 종료](https://azure.microsoft.com/updates?id=570283)
2029년 9월 30일 공식 지원 종료 예정, 대안으로 Arc-enabled Servers 등 전환 가이드 제공, 마이그레이션 안내 적극 지원.

### [Azure IoT Central 2029년 9월 20일 지원 종료](https://azure.microsoft.com/updates?id=569914)
IoT Central 대신 IoT Hub, DPS, Microsoft Fabric 등 전환 권장, playbook·파트너 매핑, 고객 지원 및 기술 안내 상세 제공.

### [Dv3/Dsv3/Ev3/Esv3 VM 시리즈 지원 종료](https://azure.microsoft.com/updates?id=572346)
2029년 11월 15일 대규모 VM 시리즈 퇴출, 최신 v5 시리즈로 조기 마이그레이션 권장, 비용·엔지니어링 효율 안내 병행.