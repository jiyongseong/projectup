# Azure 주간 업데이트 요약 - 2026-01-26

## 🚀 정식 지원
Azure에서는 여러 서비스에 대한 정식 지원을 발표하며, 운영 효율성과 사용자 경험을 강화하는 다양한 기능이 추가되었습니다. AKS는 Ubuntu 24.04 OS 지원을 통해 OS 마이그레이션을 간편하게 할 수 있도록 지원하며, Azure NAT Gateway는 향상된 네트워크 성능과 듀얼 스택 지원을 제공합니다. 이외에도 Playwright Workspaces 보고 기능이 추가되어 디버깅 작업을 더욱 활용 가능하도록 했습니다.

### [Ubuntu 24.04 지원 (AKS)](https://azure.microsoft.com/updates?id=548096)
AKS 클러스터에서 Ubuntu 24.04 OS 지원이 도입되었으며, OS SKU를 사용하여 유연한 마이그레이션 및 클러스터 운영이 가능하게 되었습니다.

### [StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=547772)
이 새로운 NAT Gateway는 더 높은 성능과 듀얼 스택 연결성을 제공하며, Zone-redundant 기능으로 안정성을 증대시킵니다.

### [Playwright Workspaces 테스트 보고](https://azure.microsoft.com/updates?id=550379)
Playwright Workspaces에 보고 기능이 추가되어 더 간편하고 효율적인 디버깅 환경을 제공합니다.

---

## 📦 스토리지
Azure는 데이터 중심의 확장과 지역 기반 스토리지 서비스를 강화하려고 노력하고 있습니다. Azure File Sync는 더 많은 지역에서 사용할 수 있게 되었으며, NetApp Files는 데이터 보호 및 복구를 위한 애플리케이션 볼륨 그룹 지원을 추가하여 고객 선택의 폭을 넓혔습니다.

### [Azure File Sync (이스라엘 중앙)](https://azure.microsoft.com/updates?id=548974)
Azure File Sync가 이스라엘 중앙에서도 사용할 수 있게 되어 지역 기반 데이터 요구 사항을 충족할 수 있습니다.

### [NetApp 파일 데이터 보호 볼륨 그룹](https://azure.microsoft.com/updates?id=548066)
NetApp Files는 복구 및 데이터 보호 볼륨 그룹을 통해 내구성과 안정성을 강화시켰습니다.

### [Azure File Sync 자세히 보기](https://learn.microsoft.com/en-us/azure/storage/file-sync/file-sync-introduction)
Azure File Sync의 주요 기능에 대한 자세한 정보를 확인할 수 있습니다.

---

## ⛅ 네트워킹
네트워킹 측면에서 StandardV2 NAT Gateway의 정식 지원이 중요한 업데이트로 포함되었습니다. Zone Redundancy 및 듀얼 스택 지원이 포함된 이 새로운 기능은 네트워크 안정성과 성능을 극대화합니다. 또한, 네트워크 관리자가 연결성을 보다 체계적으로 관리할 수 있는 로깅 기능도 도입되었습니다.

### [Zone-redundant StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=547772)
Zone Redundancy, 높은 처리량, 듀얼 스택 지원 등 다양한 기능으로 네트워킹을 강화합니다.

### [Azure Switzerland North의 테스트 서비스](https://azure.microsoft.com/updates?id=550685)
Azure Load Testing이 스위스 북부 지역에서도 사용 가능해져 글로벌 연결성을 확대합니다.

### [Azure NAT Gateway 자세히 보기](https://learn.microsoft.com/en-us/azure/nat-gateway/nat-overview#standardv2-nat-gateway)
새로운 NAT Gateway의 세부사항 및 이점에 대해 알아보세요.

---

## 🤖 개발 도구 및 DevOps
Azure의 개발 도구와 DevOps는 더욱 강력해졌습니다. 로드 테스트와 보고 기능이 통합되면서 전체 개발 및 테스트 주기를 효율적으로 관리할 수 있습니다. 자동화된 워크플로와 보고 대시보드로 프로젝트 성과를 극대화할 수 있습니다.

### [CI/CD 통합 로드 테스트](https://azure.microsoft.com/updates?id=550685)
Azure Load Testing은 CI/CD 워크플로에 통합되어 테스트를 자동화하고 성능 문제를 빠르게 식별할 수 있습니다.

### [Playwright Workspace 보고](https://azure.microsoft.com/updates?id=550379)
테스트 디버깅을 위한 통합 보고 기능이 도입되며 효율성이 향상되었습니다.

### [Azure Load Testing 리소스 보기](https://aka.ms/malt-resources)
로드 테스트 사용에 대해서 더 많은 정보를 알아볼 수 있습니다.

---

## ☸️ 컨테이너 및 Kubernetes
Azure Kubernetes Service(AKS)는 보안 강화 및 운영 효율성을 높이는 다양한 업데이트를 도입했습니다. Ubuntu 24.04 지원을 통해 OS 업그레이드가 간소화되었으며, Deployment Safeguards를 통해 클러스터 보안이 강화되었습니다.

### [AKS의 Ubuntu 24.04 지원](https://azure.microsoft.com/updates?id=548096)
Ubuntu 24.04 지원으로 AKS 클러스터에서 최신 OS로 마이그레이션할 수 있습니다.

### [Deployment Safeguards](https://azure.microsoft.com/updates?id=548101)
Pod Security Standards를 도입하여 클러스터 전체의 배포 보안을 간소화하고 강화했습니다.

### [Ubuntu OS 업그레이드 알아보기](https://aka.ms/aks/upgrade-os-version)
Ubuntu OS 버전에 대한 자세한 업데이트 및 마이그레이션 정보를 확인해보세요.