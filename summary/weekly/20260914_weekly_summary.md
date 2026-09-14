# Azure 주간 업데이트 요약 - 2026년 09월 14일

## 🚀 신규 기능 및 정식 지원
지난주 Azure는 주요 서비스의 정식 지원과 기능 개선을 통해 운영 효율성과 보안, 개발자의 편의성을 대폭 향상시켰습니다. Azure Copilot Troubleshooting Agent가 정식 지원됨에 따라 운영자가 운영 이슈를 탐지 및 해결하는 과정이 더욱 통합되고 간편해졌으며, 개발자 CLI 확장 프레임워크의 정식 지원은 각 조직 맞춤 개발·배포 자동화를 자유롭게 설정할 수 있게 했습니다. VM/VMSS용 Ephemeral OS Disk의 전체 캐싱 기능은 I/O 민감형 작업에서 10배 빠른 디스크 성능을 제공하여 AI, 실시간 분석, 대규모 서비스에 최적화된 환경을 구현합니다. 사용자 인증 보안이 크게 강화된 SAS 기능과 Playwright Workspaces의 리전 확대도 개발·운영의 편의성과 신뢰도를 높였습니다. 이러한 신규/개선 기능들은 Azure 플랫폼이 제공하는 클라우드 서비스의 경쟁력을 한 단계 끌어올렸습니다.

### [Azure Copilot Troubleshooting Agent 정식 지원](https://azure.microsoft.com/updates?id=570980)
운영 환경에서 발생하는 이슈 탐지와 해결을 통합적으로 관리할 수 있도록 Copilot 내장 트러블슈팅 에이전트가 정식 지원됩니다.

### [Ephemeral OS Disk full caching VM/VMSS 정식 지원](https://azure.microsoft.com/updates?id=570551)
가상 머신 및 VM 스케일 세트에서 OS 이미지 전체를 캐싱하여 실시간·AI 워크로드 등 I/O 민감형 작업에서 획기적으로 빠른 성능과 장애 내구성이 제공됩니다.

### [User-bound SAS Azure Storage 정식 지원](https://azure.microsoft.com/updates?id=569241)
Entra ID 기반 사용자-위임 SAS 토큰으로 외부 접근이 특정 사용자로 한정되어 인증과 보안이 크게 강화되었습니다.


## ⚙️ 개발 도구 및 DevOps
Azure의 개발자 환경과 DevOps 워크플로우가 한층 강화되었습니다. Azure Developer CLI 확장 프레임워크의 정식 지원은 별도 플러그인과 맞춤형 도구를 자유롭게 연동해, 조직별 개발의 자동화 및 효율적인 배포 프로세스 구축이 가능합니다. Playwright Workspaces 지원 리전이 확대되어 대규모 브라우저 테스트, 디버깅, CI/CD 연계가 더욱 쉽고 안전하게 이루어집니다. Azure Functions Flex Consumption 플랜에 TLS/SSL과 End-to-End TLS 암호화 기능이 추가되어, 서버리스 환경에서도 인증 및 트래픽 암호화가 완전하게 지원됨으로써 보안성이 대폭 향상되었습니다. 이번 개선으로 개발·테스트·배포 사이클에서 보안과 생산성이 모두 업그레이드되었으며, 다양한 클라우드 서비스와의 연계도 한층 견고해졌습니다.

### [Azure Developer CLI 확장 프레임워크 정식 지원](https://azure.microsoft.com/updates?id=570881)
CLI의 확장성과 자동화 도구 연계를 통해 조직별 맞춤형 개발 워크플로우 구축이 가능해졌습니다.

### [Playwright Workspaces 리전 확대 정식 지원](https://azure.microsoft.com/updates?id=570919)
스위스 북부, 일본 동부, 호주 동부 리전에서 Playwright 테스트 환경이 정식 지원되며, CI/CD 등 개발자 테스트 환경을 대규모로 확장할 수 있습니다.

### [Azure Functions Flex Consumption TLS/SSL 및 암호화 지원](https://azure.microsoft.com/updates?id=570940)
TLS/SSL 인증서 및 엔드투엔드 암호화 지원으로 서버리스 환경에서도 안전한 사용자 인증과 트래픽 보안이 가능합니다.


## 🗄️ 스토리지 및 데이터 마이그레이션
Azure Storage는 보안 및 데이터 이관 기능이 크게 향상되었습니다. 사용자-기반 SAS 기능의 정식 지원으로 Entra ID 인증 기반 SAS 토큰이 제공되어 외부 접근이 특정 사용자로 제한됩니다. Storage Mover의 온프레미스 SMB 파일 공유 Azure Files 에이전트리스 마이그레이션 미리 보기 기능은 별도의 온프레미스 에이전트 없이 데이터 이전이 가능하며 Key Vault 연동으로 인증 보안을 보장합니다. REST API를 활용한 사용자 위임 SAS를 통해 개발자들이 보다 쉽게 보안 인증 토큰을 관리할 수 있습니다. 이번 업데이트는 하이브리드·클라우드 환경의 데이터 이관을 보다 안전하고 편리하게 지원하며, 온프레미스와 Azure Files 간 마이그레이션 효율성을 대폭 높였습니다.

### [User-bound SAS Azure Storage 정식 지원](https://azure.microsoft.com/updates?id=569241)
Azure Blobs, Files, Tables, Queues에서 Entra ID 기반 사용자 인증 SAS 토큰을 활용하여 데이터 접근 권한을 강력하게 제한할 수 있습니다.

### [온프레미스 SMB 파일 공유 Azure Files 에이전트리스 마이그레이션 미리 보기](https://azure.microsoft.com/updates?id=570910)
에이전트가 필요 없는 온프레미스 Windows Server, NAS 데이터의 Azure Files 마이그레이션이 미리 보기로 지원되며, Key Vault를 통한 보안 인증도 강화되었습니다.

### [Azure Storage에서 사용자 위임 SAS 생성 방법](https://learn.microsoft.com/rest/api/storageservices/create-user-delegation-sas)
REST API를 이용해 보안성이 높은 사용자 위임 SAS를 생성 및 관리하는 방안을 공식 문서로 제공합니다.


## 🏗️ 인프라 및 컴퓨트
인프라와 컴퓨트 영역에서는 Ephemeral OS Disk의 전체 캐싱 기능 정식 지원이 주요한 변화입니다. VM과 VMSS의 OS 이미지를 로컬 스토리지에 전체 캐싱하여 고성능 부팅, 빠른 I/O, 높은 내구성을 보장합니다. Azure Functions Flex Consumption 플랜에 TLS/SSL 및 트래픽 암호화 지원이 추가되어 보안성이 크게 강화되었으며, CLI 및 자동화 도구 확장성 역시 인프라 운영 효율성을 높이고 개발자의 생산성을 향상시켰습니다. 이번 변화로 대규모 데이터 분석, AI 학습, 실시간 서비스 및 서버리스 환경에서 민첩한 운영과 장애 대응이 강화되었습니다.

### [Ephemeral OS Disk full caching VM/VMSS 정식 지원](https://azure.microsoft.com/updates?id=570551)
OS 이미지를 전체 캐싱해 I/O 민감형 워크로드에서 최상의 성능과 장애 내구성을 제공합니다.

### [Azure Functions Flex Consumption TLS/SSL 및 암호화 지원](https://azure.microsoft.com/updates?id=570940)
Flex Consumption 플랜에 TLS/SSL, 엔드투엔드 암호화 지원이 추가되어 서버리스 플랫폼 보안이 한층 강화되었습니다.

### [Azure Developer CLI 확장 프레임워크 정식 지원](https://azure.microsoft.com/updates?id=570881)
개발 및 배포 자동화 도구의 확장성으로 인프라 운영과 개발 환경 혁신이 구현되었습니다.


## 🛑 지원 종료 및 사용 중단 안내
2026년 12월 10일부터 AKS에서 Azure Linux with OS Guard의 지원이 종료됩니다. 이후 기존 노드풀에 대한 보안 패치, 이미지 제공, 리이미지 및 재배포가 중단되며, 2027년 3월 10일에는 해당 노드 이미지도 완전히 제거됩니다. 이미지는 마이그레이션 가이드로 Azure Container Linux로 이전할 수 있으며, 기존 워크로드의 중단 없는 이전과 검증이 중요합니다. 관련 커뮤니티 및 공식 문서를 통한 지원 옵션도 제공될 예정입니다. 최신 OS 운영 환경으로 전환하지 않을 경우, 서비스 안정성과 보안에 영향이 있으니 반드시 마이그레이션을 준비해야 합니다.

### [AKS Azure Linux with OS Guard 지원 종료 안내](https://azure.microsoft.com/updates?id=571257)
2026년 12월 10일부터 신규 노드 풀 생성 및 이미지 배포, 보안 패치 지원 등이 중단되어 서비스 전환이 필요합니다.

### [Azure Container Linux로 노드 마이그레이션 가이드](https://learn.microsoft.com/en-us/azure/azure-linux/tutorial-migrate-azure-container-linux-aks)
기존 OS Guard 노드풀을 Azure Container Linux로 안전하게 이전할 수 있도록 공식 마이그레이션 방법이 제공됩니다.

### [AKS 지원 종료 관련 커뮤니티 Q&A](https://docs.microsoft.com/answers/topics/25346/azure-kubernetes-service.html)
지원 종료와 마이그레이션 관련 질의응답은 Microsoft Q&A 및 GitHub 커뮤니티에서 전문가와 상담·가이드가 가능합니다.