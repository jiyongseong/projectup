# Azure 주간 업데이트 요약 - 2026년 10월 19일

## 🔒 보안 및 관리
지난주 Azure에서는 HSM 하드웨어 감사 로깅, 외부 키 관리 기능, Azure Site Recovery의 ARC 통합 등 보안 및 관리 역량이 크게 강화되었습니다. 하드웨어 기반 감사 로깅은 HSM 관리 작업에 대해 서명된 무결성 기록을 제공하여 조직의 보안 모니터링, 규정 준수 보고, 포렌식 조사 효율을 높입니다. 외부 키 관리 기능은 규제와 데이터 주권 요구를 충족하며, 고객 인프라 내 자체 HSM 장비에서 키를 직접 관리할 수 있도록 지원합니다. ARC 활성화된 Windows VMWare VM 및 물리 서버에 대한 Site Recovery 지원은 온프레미스와 멀티클라우드 환경의 재해 복구 구성을 확장하여, 거버넌스와 운영 효율성이 향상되었습니다. 전체적으로 보안, 감사, 규정 준수, 효율적 운영을 위한 기반이 한층 견고해진 한 주였습니다.

### [Azure Cloud HSM 하드웨어 감사 로깅](https://azure.microsoft.com/updates?id=576377)
하드웨어 기반 감사 기록을 통해 인증 및 무결성 검증이 가능해졌으며, Azure Monitor Log Analytics와 연동하여 보안과 운영 시나리오에 적용할 수 있습니다.

### [Azure Site Recovery: ARCEnabled Windows VMWare/Physical 서버 지원](https://azure.microsoft.com/updates?id=576214)
Azure ARC로 관리되는 온프레미스 및 VMWare 환경의 Windows 서버에 Site Recovery를 적용해 클라우드 기반 재해 복구 시나리오를 확장할 수 있습니다.

### [Azure Key Vault Managed HSM 외부 키 관리 정식 지원](https://azure.microsoft.com/updates?id=574296)
규제 요건 고객이 키 암호화 키를 자체 HSM 장비에 보관할 수 있게 하여, Microsoft 외부에서 키 제어가 이루어집니다.


## 🕸️ 네트워킹 및 인프라
이번 주에는 네트워크 접근성 및 인프라 안정성 강화를 위한 새로운 기능들이 등장했습니다. 표준 서비스 엔드포인트는 공용 IP 인스턴스를 식별자로 활용해 여러 서브넷과 네트워크 간 연결을 지원하고, 기존 엔드포인트의 확장성과 관리 문제를 해소했습니다. 이를 통해 PaaS 자원에 견고한 접근제어가 가능하며, 네트워크 경계 내에서 논리적 보안 구성을 구축할 수 있습니다. VM 스케일셋의 영역 자동 균형 기능은 각 영역의 VM 수를 실시간 모니터링하고 배분함으로써 장애 발생 시 한 영역에 집중된 위험을 효과적으로 줄일 수 있습니다. 공식 문서와 가격 정책 업데이트로 관리 및 운영의 투명성이 높아졌으며, 네트워크와 인프라의 복잡성을 줄여주는 한 주가 되었습니다.

### [표준 서비스 엔드포인트](https://azure.microsoft.com/updates?id=571025)
Azure Private Link 패밀리의 신규 기능으로, 공용 IP 인스턴스를 통해 여러 서브넷·가상 네트워크 연결 및 보안 경계 구성이 가능합니다.

### [Virtual Machine Scale Sets 영역 자동 균형 정식 지원](https://azure.microsoft.com/updates?id=576334)
장애 상황 발생 시 VM 인스턴스 배치를 자동 조정해 단일 영역 장애의 리스크를 최소화하고, 애플리케이션 안정성을 높입니다.

### [표준 서비스 엔드포인트 기능 상세 문서](https://azure.microsoft.com/updates?id=571025)
기능 구조와 보안 경계 설정, 가격 정책 등 세부 정보를 공식 문서를 통해 확인할 수 있습니다.


## 💾 스토리지 및 데이터 관리
스토리지 영역에서는 Azure Storage Mover를 활용한 파일 데이터 교차 지역 복사 및 동기화 기능이 미리 보기로 출시되었습니다. 이 기능을 통해 Azure Files의 스토리지 계정 간, 리전 간, 구독 간 데이터 복사와 동기화가 자동화되며 SMB 공유도 지원합니다. 비즈니스 연속성, 다중지역 백업, 분석 시스템 데이터 배치 등 다양한 시나리오에 적용할 수 있습니다. 중앙화된 스케줄링과 모니터링, 감사, 메타데이터 보존이 포함되어 반복적인 파일 이동 및 백업을 효율적으로 관리할 수 있습니다. 관리 편의성과 데이터 신뢰성, 다양한 클라우드 전략을 지원하는 중요한 변화였습니다.

### [Azure Files 교차 지역 데이터 복사 및 동기화 (미리 보기)](https://azure.microsoft.com/updates?id=576542)
Azure Storage Mover를 사용해 스토리지 계정 간, 리전 간, 구독 간 파일 데이터 복사·동기화가 자동화됩니다.

### [Azure Storage Mover 교차 파일 복사 미리 보기 시작하기](https://learn.microsoft.com/en-us/azure/storage-mover/azure-files-to-azure-files-copy)
SMB 공유 대상 파일 이동 및 복사 방법을 공식 문서에서 안내합니다.

### [Azure Storage Mover 서비스 소개](https://learn.microsoft.com/en-us/azure/storage-mover/service-overview)
데이터 이동, 관리, 자동화 서비스의 전체 구조와 특징을 설명합니다.


## 🧠 AI & Analytics
AI 및 분석 영역에서는 Azure Databricks의 사설 네트워크 게이트웨이 미리 보기 출시가 주요 이슈였습니다. 이 기능은 서버리스 컴퓨트 환경이 사설 네트워크 또는 방화벽과 연동될 수 있도록 해, 네트워크 트래픽 제어와 출처 IP 식별을 간소화합니다. NCC 및 Private Link와 조합하면 한층 더 안전하고 유연한 데이터 분석 및 머신러닝 워크로드 환경을 구축할 수 있습니다. Databricks 운영자들은 네트워크 연결성 강화로 개인정보 보호 및 보안 요구에 좀 더 쉽게 대응할 수 있게 되었으며, 전반적으로 데이터 분석 플랫폼과 서비스의 통합 및 보안 확장성이 강조되었습니다.

### [Azure Databricks 사설 네트워크 게이트웨이 (미리 보기)](https://azure.microsoft.com/updates?id=576556)
서버리스 컴퓨트가 고객 VNet과 방화벽을 통해 사설 리소스에 안전하게 접근할 수 있어 네트워크 보안이 강화되었습니다.

### [Databricks 사설 네트워크 게이트웨이 공식 문서](https://learn.microsoft.com/en-us/azure/databricks/security/network/serverless-network-security/private-network-gateway)
해당 게이트웨이의 서비스 구조 및 네트워크 연결 설정 방법을 안내합니다.

### [Azure Databricks 네트워크 연결성 강화](https://azure.microsoft.com/updates?id=576556)
NCC 구성 및 Private Link와의 결합으로 다양한 보안 시나리오에 적용이 가능합니다.


## 🌏 기타 주요 기능 업데이트
기존 카테고리에 포함되지 않은 주요 업데이트들은 Azure 서비스의 사용성과 관리 편의성을 높이고 있습니다. 관리형 리소스 자동화, 서비스 엔드포인트 가격 정책, API 및 클라이언트 툴 신기능 등 다양한 영역에서 실질적인 운영 효율 향상이 있었으며, 고객 클라우드 환경의 실제 적용이 더 쉬워졌습니다. 특히 신규 기능의 과금 체계와 운영 비용 정보를 투명하게 제공하고, 자동화 기능과 상세 문서로 고객의 서비스 활용도를 높였습니다. 이번 주 기타 기능들은 인프라와 네트워크 기능 확장뿐 아니라, 재해 복구·운영 자동화에 실질적 도움을 주는 업데이트였습니다.

### [Azure Private Link 표준 서비스 엔드포인트 가격 정책](https://azure.microsoft.com/en-us/pricing/details/private-link/)
신규 기능의 과금 체계와 운영 비용을 명확히 확인할 수 있습니다.

### [VM 스케일셋 영역 자동 균형 기능 활성화 및 문서](https://aka.ms/AutoZoneBalanceDocs)
VM 스케일셋에 신규 자동 균형 기능을 적용하는 방법 및 API, CLI 활용법을 안내합니다.

### [Site Recovery ARC 지원 상세 안내](https://learn.microsoft.com/en-us/azure/site-recovery/feature-updates-whats-new#azure-site-recovery-support-for-azure-arc-enabled-windows-vmwarephysical-servers)
Site Recovery ARC 지원 신규 기능과 실제 적용 예제까지 공식 문서에서 자세히 소개합니다.