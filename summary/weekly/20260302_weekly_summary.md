# Azure 주간 업데이트 요약 - 2026년 03월 02일

## 🚀 출시 및 정식 지원 업데이트

Azure 플랫폼은 사용자 경험과 데이터 관리 효율성을 강화하기 위해 여러 새로운 기능을 도입했습니다. 특히 Azure Red Hat OpenShift의 지역 확장과 Azure SQL의 유용한 기능 업데이트가 주목받았습니다. Azure Red Hat OpenShift는 말레이시아 서부, 뉴질랜드 북부, 멕시코 중부 지역에서 정식 지원을 시작했으며, 이는 데이터 레지던시 및 규제 요구 사항을 충족시키면서도 안정적인 쿠버네티스 환경을 제공합니다. 또한 Azure SQL의 MSSQL 확장 기능은 검색 및 통합 옵션 추가로 개발자 경험을 더욱 심화시켰습니다.

### [Azure Red Hat OpenShift, 신규 지역 정식 지원](https://azure.microsoft.com/updates?id=557897)
말레이시아 서부, 뉴질랜드 북부, 멕시코 중부에서 Azure Red Hat OpenShift가 정식 지원을 시작하며, 사용자 데이터와 가까운 위치에서 성능 최적화를 제공하여 생산성을 높였습니다.

### [Azure SQL, MSSQL 확장 기능 업데이트](https://azure.microsoft.com/updates?id=557517)
MSSQL 확장 기능으로 검색 기능 및 설정 가져오기 기능이 추가되어 SQL 데이터베이스 관리가 더욱 간편해졌습니다.

### [MSSQL용 설정 및 키보드 단축키 통합](https://aka.ms/vscode-mssql-february2026)
Visual Studio Code에서 MSSQL 확장을 통해 사용 가능한 단축키와 설정 가져오기가 지원되어 개발자 편의성이 확대되었습니다.

---

## 🔍 미리 보기 기능 및 개선사항

Azure는 데이터베이스 및 보안 관련 미리 보기 기능을 통해 혁신적인 업데이트를 제공했습니다. Azure PostgreSQL의 지리적 백업 기능은 데이터 안전성을 강화하며, Azure Monitor와 애플리케이션 게이트웨이 WAF의 신규 기능은 보안 및 분석 능력을 높이는 데 주력하고 있습니다. 이러한 미리 보기 기능은 작지만 중요한 사용 사례를 커버하여 시스템 안정성과 보안을 크게 향상합니다.

### [지리적 백업, Azure PostgreSQL Premium SSD v2](https://azure.microsoft.com/updates?id=557532)
지리적 백업으로 재난 복구 능력을 향상시키고, 주요 데이터 손실을 방지하기 위한 도구와 옵션을 제공합니다.

### [스토리지 보안 강화, SAS와 Entra ID](https://learn.microsoft.com/rest/api/storageservices/create-user-delegation-sas)
SAS 토큰과 Entra ID를 결합한 새로운 인증 방식으로 스토리지 보안을 한층 강화하고 관리의 유연성을 높였습니다.

### [애플리케이션 게이트웨이 WAF Insights](https://azure.microsoft.com/updates?id=557416)
공격 패턴 분석 기능과 필터 설정이 강화된 WAF Insights로 네트워크 보안과 트러블 슈팅 능력이 확장되었습니다.

---

## 🗑️ 지원 종료 및 사용 중단 알림

특정 솔루션 및 시스템의 지원 종료로 기존 플랫폼을 최신 대안으로 전환해야 하는 시점이 다가왔습니다. 이번 주에는 NGINX Ingress와 Windows Server Annual Channel 관련 주요 지원 종료 내용이 포함되어 사용자들에게 미리 알려주고 있습니다. 이를 통해 전환 작업을 조기에 시작하여 운영 중단을 예방할 수 있습니다.

### [NGINX Ingress, 애플리케이션 라우팅 지원 종료](https://azure.microsoft.com/updates?id=555839)
2026년 11월까지 NGINX Ingress 지원이 종료되며, Gateway API 및 Application Gateway 같은 대안 솔루션으로 전환할 것을 권장합니다.

### [Windows Server Annual Channel 사용 중단 예정](https://azure.microsoft.com/updates?id=557224)
Windows Server Annual Channel은 곧 서비스 종료되며 Long Term Servicing Channel(LTSC)로 마이그레이션 필요성이 대두됩니다.

### [Windows 노드 업그레이드 가이드](https://learn.microsoft.com/azure/aks/upgrade-windows-os)
Windows Server 노드의 업그레이드 과정을 간단하게 설명한 마이그레이션 가이드는 전환 과정에서 필수적인 정보를 제공합니다.

---

## 📦 컨테이너 및 Kubernetes 서비스 관련 업데이트

Azure는 컨테이너 및 쿠버네티스 관리의 유연성을 제공하기 위해 Azure Kubernetes Service(AKS)와 연계한 새로운 기능들을 발표했습니다. 특히 Pod 배치 조정 및 리소스 관리 정책 강화로 대규모 배치를 더 간편하게 실행할 수 있습니다.

### [Azure Monitor 파이프라인, Pod 배치 기능](http://aka.ms/AzMonpipelinePod)
AKS에서 실행되는 Azure Monitor가 리소스 집중과 배치 관리를 최적화하면서도 성능을 유지하도록 Pod 배치 설정 기능을 추가했습니다.

### [NGINX Ingress와 애플리케이션 라우팅 해설](https://learn.microsoft.com/en-us/azure/aks/app-routing)
애플리케이션 라우팅 기능을 보완하기 위한 새로운 문서가 추가되어 Ingress 활용도를 대폭 높였습니다.

### [Azure Monitor TLS 설정](https://aka.ms/AzMonTLS)
TLS/mTLS 인증을 기반으로 한 보안 강화를 통해 데이터 안전성을 높이고 고객 맞춤형 인증서를 허용합니다.

---

## 📊 네트워크 및 보안 강화

이번 업데이트는 Azure의 네트워크 환경과 데이터 보안을 개선하는 것을 목표로 악의적 활동 방지 및 분석 도구를 도입했습니다. 특히 TLS 및 mTLS 인증, 사용자 위임 SAS 업데이트는 Azure 스토리지와 네트워킹을 더욱 안전하고 강력하게 만듭니다.

### [WAF Insights, 애플리케이션 보안 강화](https://learn.microsoft.com/en-us/azure/web-application-firewall/ag/insights)
WAF Insights는 애플리케이션 게이트웨이 보안 강화를 위한 신규 도구로, 요청 필터링 및 규칙 상세 설정 기능을 제공합니다.

### [스토리지, 사용자 위임 SAS 업데이트](https://learn.microsoft.com/rest/api/storageservices/create-user-delegation-sas)
스토리지 데이터의 접근 제어와 보안 정책 설정을 강화하여 SAS 활용을 더욱 안전하게 개선했습니다.

### [TLS 및 mTLS 인증 확장](http://aka.ms/AzMonTLS)
TLS와 mTLS를 활용한 안전한 데이터 통신으로 Azure Monitor가 보안 요구 사항을 충족합니다.