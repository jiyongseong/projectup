# Azure 월간 업데이트 요약 - 2026년 08월

## 전반적인 트렌드와 핵심 인사이트

2026년 8월은 Azure 클라우드의 안정성, 보안, 확장성, 인텔리전스 강화와 운영 효율성에 중점을 둔 업데이트가 두드러진 시기였습니다. 주요 트렌드는 다음과 같이 요약할 수 있습니다.  
첫째, 정식 지원 기능의 확장과 미리 보기 기능의 공개가 눈에 띄며, 특히 컴퓨팅, 네트워킹, 데이터베이스, AI 및 관리 서비스 중심의 강화가 이루어졌습니다. 고성능 VM과 인프라, 데이터 보호 체계, 보안성 높은 네트워킹, 운영 자동화 및 시스템 관리 효율성, 클라우드 네이티브 개발환경 등이 본격적으로 확대되었습니다.  
둘째, 보안·컴플라이언스 측면에서는 VM 및 데이터베이스의 기본 보안 설정 자동화, 네트워크 경계 구조 강화 등 서비스별 보안 기능이 크게 개선되고 있습니다. Azure Firewall, Bastion, Application Gateway, WAF, Private Link 등 네트워크 보안 서비스도 성능 향상과 새로운 정책 기능 추가가 다수 이루어졌습니다.  
셋째, 데이터 및 AI의 관점에서는 Azure Databricks, AI Gateway, Genie Agents, Dragon Copilot 등 AI·분석 플랫폼의 리전 확장 및 거버넌스, 애자일 운영 경험의 대폭 개선이 주요 흐름으로 자리잡고 있습니다. Databricks Genie One 및 Agent의 무료 사용기간 연장, 중복 업데이트의 EOL 안내 등 시장 변동에 따른 대응성도 강화됐습니다.  
넷째, 개발자와 운영자의 생산성 향상을 위한 관리 및 거버넌스 기능이 대폭 업데이트되었습니다. Azure Copilot에 직접 접근 가능한 에이전트 도입, SRE Agent의 VNet 통합, Live Reports 등은 클라우드 운영 자동화와 실시간 분석에 중점을 둔 신기능입니다.  
다섯째, 새로운 기능이나 미리 보기로 제공되는 영역에서는 네트워크 이중화, IPv6 지원, Private Link 확대, SQL Database 기능, Azure Linux WSL, App Service 에이전트용 Markdown 등 클라우드 네이티브 및 하이브리드 클라우드 운영환경을 지원하는 솔루션이 빠르게 확장되고 있습니다.  
여섯째, 서비스 지원 종료 공지를 통해 시장 변화에 신속히 대응할 수 있도록 했으며, VM, 컨테이너, 모듈, 라이선스 등 주요 컴퓨팅·보안 솔루션의 퇴출 일정을 명확하게 안내합니다.  
마지막으로, Microsoft Fabric, Foundry 등 특별 카테고리별로 생태계 확장 및 플랫폼 전략이 고도화되고 있습니다.

이와 같이 이번 달의 Azure 업데이트는 ‘운영 효율성·보안성 강화’, ‘데이터·AI 플랫폼 확장’, ‘개발자 생산성 및 자동화’에 초점이 맞춰졌으며, 다양한 신규 서비스와 운영 도구, 보안 체계의 등장으로 클라우드 혁신을 견인하고 있습니다.

---

## 🖥️ 컴퓨팅 및 인프라

이번 달에는 고성능 VM, 이미지 빌더, vCore 커스터마이징, App Service 관리 인스턴스 등 컴퓨팅 환경의 대규모 확장 및 개선이 집중적으로 이루어졌습니다.  
특히 Intel Xeon 6 기반의 대형 VM, VM 이미지의 주권 클라우드 지원, 기본 보안설정 자동화 등은 엔터프라이즈·대형 워크로드의 클라우드 전환을 가속화하는 기반을 제공합니다. 또, VM 라이선스 정책 변화에 따른 대비와 운영 효율화 기능도 강화되었습니다.

### [Azure 248 및 372 vCPU D/E v7 시리즈 VM 정식 지원](https://azure.microsoft.com/updates?id=569546)
최대 372 vCPU, 2.8TiB 메모리, 400Gbps 네트워크 대역폭을 지원하는 대형 VM이 정식 출시되어 대규모 인-메모리 DB 및 대형 AI 워크로드에 적합한 환경을 제공합니다.

### [Azure VM Image Builder의 주권 및 에어갭 클라우드 지원](https://azure.microsoft.com/updates?id=570105)
Azure Government, China North 3 등 규제 클라우드에서 이미지 빌더 기능 정식 지원. 이미지 파이프라인 일관성 및 컴플라이언스 강화가 가능해졌습니다.

### [vCore 커스터마이징: SMT/HT 비활성화 및 제한 코어 설정 정식 지원](https://azure.microsoft.com/updates?id=569051)
VM의 SMT/HT 비활성화 및 코어 수 선택 기능이 추가되어 라이선스 비용 절감과 워크로드별 최적화가 가능해졌습니다.

### [Trusted Launch 기본설정 정식 지원](https://azure.microsoft.com/updates?id=568600)
Gen2 VM 및 VMSS에 Trusted Launch 기반 보안(부팅 및 vTPM 활성화) 자동 적용으로 기본 보안성이 크게 향상되었습니다.

### [Managed Instance on Azure App Service 정식 지원](https://azure.microsoft.com/updates?id=568952)
App Service에 관리 인스턴스 도입으로 온프레미스·VM 기반 앱의 PaaS 전환이 코드 수정 없이 가능해졌으며, 엔터프라이즈 .NET 워크로드에 적용 범위가 확대되었습니다.

---

## 💡 AI & 분석 플랫폼

AI 및 데이터 분석 플랫폼은 Databricks, Dragon Copilot, Unity AI Gateway의 리전 확대, 거버넌스 강화, Marketplace 채널 확장 등 다각적인 기능 보강이 집중되었습니다.  
Genie Agent 무료 사용기간 연장 및 Databricks Runtime EOL 안내 등 실무적 안내도 포함되어 있습니다.

### [Azure Databricks Lakebase 4개 리전 정식 지원](https://azure.microsoft.com/updates?id=569684)
North Central US, France Central, Germany West Central, East Asia로 Lakebase 배포 가능, 글로벌 AI/분석 워크로드의 지역적 확장 지원.

### [Unity AI Gateway 정식 지원](https://azure.microsoft.com/updates?id=568910)
Databricks 기반 AI 모델·에이전트·도구·MCP 거버넌스 일원화, 비용·접근·가드레일·모니터링 등 AI 운영 통제력 강화.

### [Dragon Copilot 의료 앱/에이전트 Marketplace 판매 채널 출시](https://azure.microsoft.com/updates?id=557775)
Microsoft Marketplace에서 Dragon Copilot 의료 앱 및 에이전트 직접 구매 가능, AI 기반 임상 및 서류 자동화 지원.

### [Azure Databricks Genie One 및 Genie Agents 무료 사용기간 연장 (2027년 1월까지)](https://azure.microsoft.com/updates?id=568964)
Genie One·Agent 무료 사용 확대 및 Genie Code/Inference SKU 할인 안내, 사용량 급증 대비 실무 지원.

### [Azure Databricks Runtime 10.4 LTS 지원 종료 예고 (2026년 11월)](https://azure.microsoft.com/updates?id=569353)
10.4 LTS 버전 EOL 일정 공개, Databricks Runtime 환경 대응 필요.

---

## 🔐 네트워킹 및 보안

네트워킹과 보안 영역에서는 Firewall, Bastion, Application Gateway, Front Door의 성능·정책 강화, Private Link 및 IPv6 지원, 경계 구조 확대 등이 두드러졌습니다.  
운영 자동화와 보안 정책 일관성, 관리성 향상이 중점적으로 이루어졌으며, 미리 보기에서 네트워크 확장·보안성 강화 신기능이 공개되었습니다.

### [Azure Firewall IDPS 성능 2.2배 최적화 정식 지원](https://azure.microsoft.com/updates?id=569256)
Firewall Premium의 TLS 검사 및 IDPS Deny 모드에서 최대 22Gbps 처리량 제공, TCP 연결당 600Mbps까지 확장.

### [Explicit Proxy in Azure Firewall 정식 지원](https://azure.microsoft.com/updates?id=568825)
Firewall Proxy 기능으로 HTTP/S 트래픽을 직접 제어, Arc 하이브리드 및 현대화 네트워크 운영에 추가적인 유연성 및 보안 제공.

### [Batch Rule 업데이트 Azure Front Door 정식 지원](https://azure.microsoft.com/updates?id=569246)
Front Door Rule 세트의 배치 관리 가능, 대형·복잡한 인프라의 규칙 일관성 및 배포 안정성 대폭 향상.

### [Application Gateway WAF의 커스텀 블록 응답코드/메시지 정식 지원](https://azure.microsoft.com/updates?id=569504)
WAF의 정책 수준 응답코드·메시지 사용자 정의 기능 도입, 보안 정책 일관성 및 유연성 강화.

### [Azure Bastion 연결 만료 설정 및 AKS 연동 정식 지원](https://azure.microsoft.com/updates?id=570020)
Bastion의 링크 만료 및 AKS API 서버 보안 연결 기능이 추가되어, 일시적 접근 및 프라이빗 클러스터 운영이 더욱 강화됨.

---

## 📊 데이터베이스 및 스토리지

DB 및 스토리지 영역에선 Azure SQL, PostgreSQL, Databricks, Azure Files, Disk Storage의 기능 개선과 운영 자동화가 중점적으로 이루어졌습니다.  
백업 불변성, 업그레이드 사전 검증, 용량 동적 확장, 워크로드별 granular 인증, 데이터 커넥터, 클라우드 네이티브 DB 운영 툴의 정식 지원이 주요 포인트입니다.

### [Azure SQL Database MSSQL 에디터 배포 및 단축키 설정 정식 지원](https://azure.microsoft.com/updates?id=569160)
MSSQL 에디터 내 구독 및 클라우드 DB 직접 생성·연결 및 ARM/Bicep/Terraform 템플릿 제공, 개발·운영 자동화 지원.

### [Azure SQL Database/Managed Instance 7일 백업 불변성 정식 지원](https://azure.microsoft.com/updates?id=568339)
최신 7일 백업 내역 기본적으로 불변성 적용, 무상 데이터 보호 강화.

### [Azure Database for PostgreSQL Flexible Server 사전 업그레이드 검증 정식 지원](https://azure.microsoft.com/updates?id=568419)
MVU(메이저 버전 업그레이드) 전 사전 검증 기능 추가, 업그레이드 실패 최소화 및 운영 예측성 개선.

### [Azure Databricks SharePoint 커넥터 정식 지원](https://azure.microsoft.com/updates?id=568905)
Lakeflow Connect 기반 SharePoint 파일 연동, 엔터프라이즈 콘텐츠와 AI 워크플로우 통합 지원.

### [Live Resize 기능, SSD v2 및 Ultra Data Disk 정식 지원](https://azure.microsoft.com/updates?id=569281)
실시간 스토리지 확장 기능으로 비용최적화 및 운영 무중단 효과 제공.

---

## 🎛️ 관리 및 운영 자동화

운영 효율화와 자동화 영역에서는 SRE Agent, Azure Copilot, App Service, Azure Route Server 등 실시간 분석 및 관리, 인프라 연결, 클라우드 거버넌스 강화가 주요 트렌드입니다.  
직관적 관리, 실시간 보고, 운영 위험 감지, 로그 처리 자동화 등이 중심입니다.

### [Azure SRE Agent 30일 체험 및 VNet 통합 정식 지원](https://azure.microsoft.com/updates?id=569760)
자동화·생성·운영 위험 감지, Runbook 연동 등 IT 운영의 인텔리전스 강화 및 보안 정책 일관성 유지.

### [Live Reports for Azure SRE Agent 미리 보기 출시](https://azure.microsoft.com/updates?id=569690)
실시간 보고서 자동화로 인시던트·운영 트렌드·건강 상태 분석 즉시 반영.

### [Azure Copilot 에이전트 직접 접근 기능 출시](https://azure.microsoft.com/updates?id=569685)
Troubleshooting·Deployment·Optimization·Resiliency 등 Copilot 에이전트 직접 채팅 접근 가능, Admin의 Granular 제어 제공.

### [Route-maps for Azure Route Server 미리 보기 출시](https://azure.microsoft.com/updates?id=568631)
경로 집약, BGP 속성 조정 등 네트워크 라우팅 제어 정교화.

### [Single-click SaaS 구매 경험 정식 지원](https://azure.microsoft.com/updates?id=568591)
Marketplace SaaS 제품 원클릭 구매 지원, 서비스 활용성 및 결제 편의성 대폭 개선.

---

## 🧩 하이브리드·멀티클라우드 및 리전 확장

ExpressRoute, VPN Gateway, VMware Solution, Private Link, Azure Site Recovery 등 하이브리드 및 멀티클라우드 확장과 지원 종료 공지, 네트워크 경계 확대가 다수 이루어졌습니다.  
네트워크/DB/스토리지 마이그레이션, 리전별 기능 확장, 라이선스 정책 변화 대응이 주요 이슈입니다.

### [Summarized Gateway Prefix Route Advertisement 정식 지원](https://azure.microsoft.com/updates?id=569743)
ExpressRoute/VPN Gateway의 경로 집약 기능으로 네트워크 환경 확장성 및 관리 효율성 향상.

### [BYON(Bring Your Own NIC) in Azure Site Recovery 정식 지원](https://azure.microsoft.com/updates?id=569515)
재해 복구 환경에서 직접 준비한 NIC 사용으로 네트워크 구성 유지 및 IP 예약 기능 제공.

### [Azure VMware Solution License-included 서비스 지원 종료 안내 (2027년 8월)](https://azure.microsoft.com/updates?id=569535)
Broadcom 라이선스 정책 변경에 기반한 서비스 퇴출 안내, 고객 BYOL로 전환 필수.

### [Azure Firewall 및 Private Link IPv6 지원 미리 보기 출시](https://azure.microsoft.com/updates?id=569520)
IPv6 기반 네트워킹 및 보안 강화, 현대형 멀티/하이브리드 클라우드 환경 대비 기능.

### [클라우드-클라우드 마이그레이션 지원 (AWS FSx에서 Azure Files로)](https://azure.microsoft.com/updates?id=567979)
Storage Mover 기반 FSx→Azure Files 무중단 마이그레이션 지원 미리 보기.

---

## 🏢 Microsoft Fabric & Foundry

Microsoft Fabric에서는 기본 Item Recovery 정책 업데이트 등 플랫폼의 데이터 보호·회복력 기능이 강화되었습니다. Foundry 카테고리에서는 플랫폼·개발 생태계의 주요 확장·개선이 지속되고 있습니다.

### [Microsoft Fabric Item Recovery 기본 활성화 공지](https://azure.microsoft.com/updates?id=569140)
Item Recovery 기능이 기본 활성화되어, 3일 기간 내 데이터 복구 지원 및 Admin 설정 변경권 제공.

---

## 🏷️ 퇴출 및 지원 종료

VM, Sentinel SAP 커넥터, Node.js, Databricks 등 서비스별 지원 종료 일정 및 대응 방안이 선제적으로 제공되었습니다.

### [Azure VMware Solution License-included 서비스 퇴출 (2027년 8월 30일)](https://azure.microsoft.com/updates?id=569535)
BYOL Mandatory, 라이선스 교체·전환 및 서비스 종료 일정 공지.

### [Microsoft Sentinel SAP 컨테이너형 커넥터 지원 종료 (2026년 9월 14일)](https://azure.microsoft.com/updates?id=568457)
Agentless 커넥터로 이관, 기존 SAP 로그 수집 종료 및 아키텍처 변경 안내.

### [Nested Confidential cc_v5 VM 지원 종료 (2026년 9월 1일)](https://azure.microsoft.com/updates?id=568661)
cc_v5 VM 시리즈 폐지, 미전환 VM 자동 종료 예정.

### [Node 22 LTS 지원 종료 (2027년 4월 30일)](https://azure.microsoft.com/updates?id=567334)
App Service Node.js 최신 버전 업그레이드 필요, 보안 업데이트 중단 및 기술 지원 종료.

### [Azure Databricks Runtime 10.4 LTS 지원 종료 (2026년 11월 1일)](https://azure.microsoft.com/updates?id=569353)
Databricks 환경 이관 권장, 작업 단절 위험 안내.

---

## 총평 및 다음 달 전망

2026년 8월 Azure 업데이트는 성능 최적화, 자동화, 보안 강화 및 관리 효율성에 집중되었습니다. 대형 워크로드 지원, AI·데이터 플랫폼의 지역적 확장, 네트워크·보안 보강, 운영 자동화·거버넌스 강화, 그리고 지원 종료 이슈에 대한 명확한 안내가 핵심입니다. 고객은 클라우드 네이티브, 하이브리드 환경, 엔터프라이즈급 요구사항에 적합한 환경을 손쉽게 구축할 수 있도록 다양한 툴과 정책이 추가되었습니다.  
다음 달에는 Azure AI·데이터 플랫폼의 신규 기능과 글로벌 리전 지원 확대, 서비스 자동화와 보안 정책 일관성 강화, 운영 위험 대응 기능 추가와 관련된 대형 업데이트가 지속될 것으로 전망됩니다. 시장 환경 변화에 따른 라이선스 정책 대응, 관리 효율화 도구의 발전, 하이브리드 클라우드 트렌드의 확대가 이어질 것입니다.