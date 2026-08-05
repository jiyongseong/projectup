# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월 Azure 업데이트는 AI·데이터·운영 혁신과 보안, 자동화 기반 IT 인프라 현대화에 집중된 흐름을 보였습니다. Kubernetes 기반 컨테이너 관리 기능 강화, AI 및 머신러닝 플랫폼의 빠른 확장, 데이터 관리와 이중화, 신뢰성 높은 인프라, 그리고 코드 실행 환경의 최신화가 두드러집니다. 기존 서비스의 지원 확장(GA), 신규 기능 출시, 지역별 데이터센터 추가 등 글로벌 확장의 동향도 주요 트렌드입니다.

특히 Azure Databricks 내 AI 모델 지원 확대(Claude Opus 5, Sonnet 5, GPT-5.6)를 통해 엔터프라이즈 수준의 AI 적용이 가속화됐고, Microsoft Foundry·Fabric 등 인텔리전스 플랫폼과의 통합이 더욱 활성화되는 모습입니다. 데이터 스토리지 및 네트워크 보안 기능(Blob Storage CRC64-NVME, Event Hubs Confidential Computing, VPN IPv6 등)은 금융·규제 산업의 요구사항에 대응한 강화 정책으로 해석할 수 있습니다.

운영 자동화 부문은 PowerShell 7.6 지원 확대, Python 3.14 도입, Runbook 환경 개선 등으로 코드 실행 환경의 최신화와 보안성 향상에 기반한 운영 효율이 부각되었습니다. Chaos Studio, Kubernetes Fleet Manager, Storage Mover 등 관리 도구의 기능 개선은 클라우드 인프라의 복원력, 이식성, 멀티클라우드 연동을 중점적으로 지원합니다.

공공과 규제 산업의 보안·컴플라이언스 요구를 반영하는 Azure Enclave, Key Vault Premium, Application Gateway/WAF 예외처리 등 기능 강화도 눈에 띕니다. 즉, Azure는 ‘개방·연동·자동화·보안·AI 기반’ 가치 실현에 충실한 플랫폼 전략을 구체화하며, 글로벌 지역별 신규 서비스와 데이터센터 오픈에 기반한 지역 확장까지 한층 강화된 모습을 보여줬습니다. 오픈소스 통합과 컨테이너 기반, DevOps 문화에 맞춘 변화가 지속적으로 이루어지고 있습니다.

---

## 🚀 신규 기능 및 서비스 출시

### 1. [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Kubernetes Gateway API를 활용한 인그레스 관리 기능이 정식 지원됩니다. 기존 ingress-nginx 기반 애플리케이션 라우팅을 11월까지 지원하며, 최신 표준에 맞춰 점진적 이전이 가능합니다.

### 2. [Azure Automation PowerShell 7.6 런북 및 런타임 환경 지원](https://azure.microsoft.com/updates?id=568102)
자동화 작업에서 PowerShell 7.6, 최신 런타임이 정식 지원되어 보안과 운영 효율을 크게 높일 수 있습니다.

### 3. [Azure Functions Python 3.14 지원](https://azure.microsoft.com/updates?id=567646)
Azure Functions에서 Python 3.14를 통해 앱 개발 시 보안, 지원 기간, 툴 호환성을 강화할 수 있습니다.

### 4. [Azure Databricks SQL Serverless UK West 출시](https://azure.microsoft.com/updates?id=567444)
UK West 지역에서 Databricks SQL Serverless가 정식 지원되어, 빠른 확장성과 자동 인프라 관리가 가능합니다.

### 5. [Azure Red Hat OpenShift Chile Central 출시](https://azure.microsoft.com/updates?id=566732)
칠레 중앙 신규 리전에서 OpenShift 서비스가 정식 지원되어 라틴아메리카 내 규제/산업용 클러스터 운영이 가능해졌습니다.

#### 카테고리 요약
이번 달은 Kubernetes 기반 네트워크 라우팅 표준 채택(Gateway API), Python·PowerShell 실행환경 최신화, SQL 워크로드 자동화, 다양한 글로벌 신규 리전 확장(칠레·UK 등)에서 클라우드 현대화·보안·효율성 강화가 두드러집니다.

---

## 🧠 AI 및 머신러닝, 데이터/분석 확장

### 1. [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
최신 AI 모델 Claude Opus 5를 Databricks에서 직접 서비스해 고도화된 추론·코딩·작업 자동화가 구현됩니다.

### 2. [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
GPT-5.6 모델을 Microsoft Foundry 구독 기반으로 Databricks에서 사용할 수 있어 데이터 중심 AI 개발 및 거버넌스 통합이 가능해집니다.

### 3. [Anthropic Claude Sonnet 5 지원](https://azure.microsoft.com/updates?id=567194)
저비용·고속 AI 모델로서 Sonnet 5가 Databricks에 연동, 대규모 코딩 및 고품질 자동화 작업이 실현됩니다.

### 4. [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
개인 식별 정보(PII) 문서 평가 기능이 한층 강화되어 데이터 보호 및 컴플라이언스 프로젝트를 신속하게 수행할 수 있습니다.

### 5. [Azure Event Hubs Dedicated Confidential Computing 지원](https://azure.microsoft.com/updates?id=567212)
메모리 내 스트리밍 데이터 보호를 위한 하드웨어 기반 보안 환경(TEE)이 제공되어 금융, 헬스케어 등 민감 데이터 처리가 안전해졌습니다.

#### 카테고리 요약
AI 모델 선택폭 증가, 데이터 안전성 확대, PII 자동 검출 및 고급 분석 기능이 Azure Databricks를 중심으로 확장되며, 클라우드 환경에서 엔터프라이즈 AI 활용을 위한 인프라가 완성되고 있습니다.

---

## ☁️ 관리 및 거버넌스, 자동화/마이그레이션

### 1. [Azure Site Recovery 5배 높은 IOPS 지원](https://azure.microsoft.com/updates?id=566966)
대량 데이터 및 고성능 워크로드의 복원력 강화로, 데이터베이스·빅데이터도 안정적으로 복구 가능합니다.

### 2. [Reservation Exchange 정책 변경 사전 안내](https://azure.microsoft.com/updates?id=568514)
2027년 2월부터 예약 서비스 교환(Exchange) 정책이 변경되어 Savings Plan 대상 서비스의 예약 교환이 제한됩니다.

### 3. [Python 2.7, 3.8 및 PowerShell 7.1/7.2 지원 종료 예고](https://azure.microsoft.com/updates?id=567556)
자동화 작업에서 낡은 런타임 버전의 지원 종료가 확정되어 최신 개발환경으로의 전환이 촉진됩니다.

### 4. [Storage Mover: GCS→Azure Blob Storage 마이그레이션 지원](https://azure.microsoft.com/updates?id=566948)
Google Cloud Storage에서 Azure Blob Storage로 네이티브 마이그레이션이 지원, 멀티클라우드 통합이 더욱 쉬워집니다.

### 5. [Chaos Studio Workspaces/Scenario 미리 보기](https://azure.microsoft.com/updates?id=567184)
리질리언스 테스트 자동화 및 앱 별 변경 관리·컴플라이언스 보고서를 신속하게 생성할 수 있습니다.

#### 카테고리 요약
자동화·운영환경의 최신화, 저장소 통합, 정책 변화 등 관리 효율성이 확대되고 체계적인 거버넌스 수립에 필요한 기능이 반영되었습니다.

---

## 🌐 네트워킹/보안/컴플라이언스

### 1. [Azure Firewall HTTP Header 삽입 지원](https://azure.microsoft.com/updates?id=568115)
HTTP/HTTPS 헤더를 방화벽 수준에서 직접 관리할 수 있어 보안·접근통제·관리 효율성이 강화됩니다.

### 2. [IPv6 지원 VPN Gateway](https://azure.microsoft.com/updates?id=567847)
IPv4/IPv6 듀얼스택 운용으로 신규 워크로드 및 네트워크 호환성 확장에 대응합니다.

### 3. [StandardV2 NAT Gateway NAT64 지원](https://azure.microsoft.com/updates?id=568409)
IPv6→IPv4 변환으로 IPv4 전용 인터넷 연동이 자연스럽게 가능해집니다.

### 4. [Azure DDoS Protection 맞춤 정책 미리 보기](https://azure.microsoft.com/updates?id=568063)
DDoS 방어 임계값 설정이 세분화되어, 유연한 보안 정책 설계가 가능합니다.

### 5. [Network Security Perimeter for Event Hubs](https://azure.microsoft.com/updates?id=567203)
플랫폼 내 논리적 경계 설정으로 데이터 유출 위험을 줄이는 네트워크 보호 기능이 강화됐습니다.

#### 카테고리 요약
네트워크 관리의 유연성 확대, 방화벽·DDoS 등 보안 기능 고도화, IPv6 지원 등 차세대 인프라 요구를 반영한 업그레이드가 집중됐습니다.

---

## 🗃️ 스토리지 및 데이터 관리

### 1. [Blob Storage CRC64-NVME 데이터 무결성 보호](https://azure.microsoft.com/updates?id=566895)
SDK 통합으로 아플리케이션에서 Storage까지 엔드-투-엔드 무결성 검증이 가능해집니다.

### 2. [Azure Files NFS EiT 지원(AKS)](https://azure.microsoft.com/updates?id=567787)
데이터 전송 암호화기능(TLS)을 Storage와 AKS간 통합하여 보안·컴플라이언스에 적합해졌습니다.

### 3. [Azure Blob Storage SFTP 엔트라 ID 인증 지원](https://azure.microsoft.com/updates?id=567085)
엔트라 ID로 SFTP 접속 관리가 기업 인증 체계와 통합되어, 보안·외부 협업 효율이 개선됩니다.

### 4. [Azure Storage Mover GCS->Blob Storage 마이그레이션 미리 보기](https://azure.microsoft.com/updates?id=566948)
데이터 이동이 자동화되어 멀티클라우드 환경에서도 스토리지 통합이 한층 손쉬워졌습니다.

### 5. [Azure NetApp Files SMB Oplocks 설정 미리 보기](https://azure.microsoft.com/updates?id=568396)
SMB 볼륨 캐싱성능을 직접 조정할 수 있어 대규모 파일 시스템 운영에 유리합니다.

#### 카테고리 요약
스토리지 무결성, 암호화·네트워크 연동, SFTP 인증 통합 등 데이터 보호·운영 호환성에 중점을 둔 기능 개선이 이뤄졌습니다.

---

## 🦾 컨테이너, Kubernetes, DevOps

### 1. [Resource Placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
다중 클러스터에 리소스 배치를 자동화하고, Azure portal로 관리 효과를 극대화 할 수 있습니다.

### 2. [Maximum Allowed Failures 기능 미리 보기](https://azure.microsoft.com/updates?id=567939)
클러스터 업데이트 실패 허용치 관리로, 대형 클러스터 운영의 복원력 전략 수립이 쉬워집니다.

### 3. [AKS Prepared Image Specification 미리 보기](https://azure.microsoft.com/updates?id=567949)
노드 이미지 사전 설정으로 컨테이너 워크로드 확장/초기화가 빨라집니다.

### 4. [Azure Functions PowerShell 7.6 미리 보기](https://azure.microsoft.com/updates?id=567651)
로컬 개발부터 Azure Functions 배포까지 PowerShell 7.6 지원이 빠르게 적용됩니다.

### 5. [Azure Chaos Studio CLI 지원 미리 보기](https://azure.microsoft.com/updates?id=567225)
CLI 기반 Chaos Studio 관리로 리질리언스 테스트가 더 자동화되고 DevOps와 쉽게 연동됩니다.

#### 카테고리 요약
컨테이너 및 Kubernetes 환경에서 자원 배치, 실패관리, 이미지최적화, CLI 확장 등 DevOps 중심 클라우드 운영 혁신이 눈에 띕니다.

---

## 💡 Microsoft Foundry 및 Microsoft Fabric

### Microsoft Foundry
#### 1. [Document PII Playground GA](https://azure.microsoft.com/updates?id=564382)
문서 기반 PII 검출 평가 기능이 강화되어 컴플라이언스 프로젝트 시행 속도가 빨라졌습니다.

#### 2. [Toolboxes 기능 정식 출시](https://azure.microsoft.com/updates?id=563481)
공유 툴 리스트 품질관리, 재사용·거버넌스 지원으로 오픈AI·연동 개발 생산성이 개선됐습니다.

#### 3. [Document PII Playground NextGen 미리 보기](https://azure.microsoft.com/updates?id=563331)
Foundry NextGen에서 샘플 문서 기반 PII 검출 적용이 가능해졌습니다.

#### 4. [단일 MCP 엔드포인트 호출 확대](https://azure.microsoft.com/updates?id=563481)
다양한 도구 및 커넥터를 하나의 엔드포인트로 호출 가능, 일관된 거버넌스 체계로 조직 내 재사용성이 높아집니다.

#### 5. [AI Gateway 미리 보기](https://azure.microsoft.com/updates?id=568184)
Foundry 및 외부 AI 자산의 보안적·거버넌스적 연동을 지원하는 AI Gateway가 API Management 영역에서 미리 보기로 출시됐습니다.

### Microsoft Fabric
#### 1. [Azure Monitor Logs 미러링 기능 미리 보기](https://azure.microsoft.com/updates?id=568322)
Log Analytics 워크스페이스 데이터를 Microsoft Fabric으로 실시간 미러링하여 비즈니스 데이터와 함께 분석이 가능해졌습니다.

---

## 🗺️ 글로벌 및 지역 확장(신규 리전/서비스)

### 1. [Azure Database for PostgreSQL India South Central 출시](https://azure.microsoft.com/updates?id=568334)
최신 리전에서 PostgreSQL Flexible Server를 사용할 수 있게 됐습니다.

### 2. [Microsoft Azure 인도 South Central 신규 리전 오픈](https://azure.microsoft.com/updates?id=568013)
AI 준비된 인프라, 데이터 주권·규제 준수 기반의 인도 내 네 번째 데이터센터 지역이 공식 출범했습니다.

### 3. [Azure Red Hat OpenShift Chile Central 출시](https://azure.microsoft.com/updates?id=566732)
칠레 신규 리전을 통해 OpenShift 클러스터를 라틴아메리카에 직접 구축할 수 있습니다.

### 4. [강화된 지역별 서비스 및 규제 대응 지원](https://azure.microsoft.com/updates?id=568013)
로컬 인프라·규제 맞춤 인프라 및 데이터 주권 준수 중심의 확장 정책이 강조되었습니다.

### 5. [Azure Chaos Studio 글로벌 지원 기능 확대](https://azure.microsoft.com/updates?id=567184)
앱별 장애 시나리오 자동화·리질리언스 강화가 전 세계적 Azure 워크로드에 실제로 적용되고 있습니다.

#### 카테고리 요약
신규 리전 확대, 로컬 특화 클라우드 인프라 지원, 규제산업 맞춤 데이터센터 준수가 글로벌 Azure 확대를 견인합니다.

---

## 총평 및 다음달 전망

이번 달 Azure 업데이트는 AI 모델 다양성 강화, 관리 자동화와 운영 편리성 도약, 네트워크·스토리지 보안 강화, 글로벌 신규 리전 확장 등 전방위적인 진화 양상을 보여줬습니다. AI·데이터·운영 혁신과 신뢰성, 복원력, 보안 및 컴플라이언스가 모든 업데이트의 중심을 이루며, 위협 대응과 엔터프라이즈 요구에 최적화된 기능 변화를 꾸준히 이어가고 있습니다.

다음 달에는 Foundry, Fabric 등 지능형 플랫폼 간 연동성, 글로벌 지역별 전문화된 기능 추가, DevOps와 AI 자동화가 더욱 심화될 전망입니다. 또한, 기존 리전의 서비스 업그레이드, 데이터 보안/암호화 정책 강화, 오픈소스 커뮤니티 협력 확대 등을 통해 엔터프라이즈 클라우드 환경의 운영 효율성과 유연성이 한층 진화할 것으로 기대됩니다.