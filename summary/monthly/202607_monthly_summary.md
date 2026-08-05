# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드 및 핵심 인사이트

2026년 7월 Azure 업데이트는 클라우드 혁신과 AI 융합에 대한 Microsoft의 전략이 본격화된 시점을 보여줍니다. 이번 달은 인프라 확장, 보안 강화, AI/머신러닝 기능의 대폭 향상, 데이터 관리 효율화, DevOps 통합 가속, 멀티클라우드 지원, 그리고 플랫폼의 지속적인 자동화와 관리 방식 개선이 두드러집니다.

특히 정식 지원(GA)된 업데이트가 대다수에 달하며, 다음과 같은 흐름이 뚜렷합니다:

- **AI 및 데이터 플랫폼 강화:** Azure Databricks 등 주요 서비스에서 Claude Opus 5, Sonnet 5, OpenAI GPT-5.6 등 최신 모델이 도입되어 엔터프라이즈 데이터 분석과 AI 애플리케이션이 매우 용이해졌습니다. Microsoft Foundry 역시 조직 전체에 AI 도구를 손쉽게 적용할 수 있는 툴박스 기능을 정식 지원하며, 문서 기반 PII 탐지 등 실무적 AI 서비스 확대가 진행되고 있습니다.
- **운영 자동화 및 관리 효율화:** PowerShell 7.6 런북 및 Azure Chaos Studio, Kubernetes Fleet Manager의 리소스 배포 등 자동화와 관리가 더욱 세분화되고, 효율적으로 진화하고 있습니다.
- **보안·컴플라이언스 수준 향상:** Confidential Computing 도입과 Blob Storage의 데이터 무결성 강화, Entra ID 기반 SFTP, 네트워크 보안 강화(NSP 등), Azure Firewall의 헤더 삽입 등 보안 기능들이 확장되고 있습니다. 이제 데이터의 전송 경로, 저장, 처리 전반에 걸쳐 보안/컴플라이언스가 자동화되어 제공됩니다.
- **멀티클라우드·하이브리드 전략 확대:** Azure Storage Mover를 통한 Google Cloud 데이터 마이그레이션, Kubernetes 기반 하이브리드 컨테이너 관리 기능 등이 출시되어 다양한 환경의 클라우드 통합이 더 쉬워졌습니다.
- **인프라 및 네트워크 혁신:** 새로운 클라우드 리전(인도 South Central, 칠레 Central) 개설, IPv6 지원, NAT64, Azure Kubernetes Fleet 관리, Prepared Image Specification 등 인프라의 확장과 네트워크 현대화가 진행되고 있습니다.
- **DevOps/관찰성 진화:** Azure Monitor Logs의 Microsoft Fabric 연동 및 애플리케이션 인사이트 내 AI 텔레메트리 보호, Chaos Studio 시나리오 도입 등 개발 및 운영자가 현황과 리스크를 한눈에 파악할 수 있는 환경이 강화되고 있습니다.
- **서비스 사용성 및 확장:** PowerShell, Python 런타임의 지속적인 지원 및 사용 중단 안내, Azure넷앱 파일 등의 기능 확장이 실제 개발과 운영에서 효율성과 안정성을 동시에 추구하도록 설계되고 있습니다.

이번 달 Azure는 전방위적인 혁신과 확장에 초점을 맞추며, AI·데이터·보안·관리·운영 자동화 등 모든 영역에서 ‘클라우드 퍼스트 조직’을 위한 최적화된 플랫폼을 제공했습니다.


---

## 🖥️ 컴퓨트, 컨테이너, 네트워크

이번 달 컴퓨트 및 네트워크 분야의 변화는 현대적 클라우드 환경의 확장과 실무적 배치 효율화가 중심입니다.

1. [Application Routing with Gateway API 정식 지원](https://azure.microsoft.com/updates?id=567944)  
AKS에서 Gateway API 기반 애플리케이션 라우팅을 도입하여 서비스 메시를 사용하지 않고도 표준적, 경량화된 인그레스 관리가 가능합니다. 기존 nginx 기반 모델도 11월까지 지원되어 단계적 마이그레이션이 가능합니다.

2. [Resource placement in Azure Kubernetes Fleet Manager 정식 지원](https://azure.microsoft.com/updates?id=567931)  
플릿 내 여러 AKS 및 Arc 클러스터에 리소스를 일괄 배치하는 기능이 GA로 출시, 대규모 Kubernetes 환경의 관리 효율이 크게 증가했습니다.

3. [Prepared Image Specification 미리 보기](https://azure.microsoft.com/updates?id=567949)  
AKS 노드 이미지 사전 준비 기능으로 AI, GPU 등 성능 민감 워크로드의 노드 스타트업 속도가 빨라지고, 확장 타이밍의 예측성이 향상되었습니다.

4. [IPv6 지원 for Azure VPN Gateway 정식 지원](https://azure.microsoft.com/updates?id=567847)  
IPv6 트래픽을 VPN 터널로 처리할 수 있게 되어, 듀얼스택 및 네트워크 현대화에 대응할 수 있습니다.

5. [NAT64 on StandardV2 NAT Gateway 정식 지원](https://azure.microsoft.com/updates?id=568409)  
NAT64 기능을 통해 IPv6 워크로드가 IPv4 전용 인터넷 서비스와 연동 가능해져 클라우드 네트워크 호환성이 강화되었습니다.

이번 달 네트워크/컴퓨트 업데이트는 대규모 하이브리드·멀티클라우드 환경의 효율적인 관리와, 네트워크 현대화, 확장성 확보가 핵심입니다.


---

## 🗄️ 데이터, 분석, AI·머신러닝

Azure의 데이터 및 AI 생태계는 차세대 모델 도입과 연동성 증대에 중점을 두었습니다.

1. [Claude Opus 5 on Azure Databricks 정식 지원](https://azure.microsoft.com/updates?id=568316)  
최신 Opus 5 모델이 Databricks에서 AI Model Serving을 통해 이용 가능, 고난이도 추론 및 코딩 작업, 워크플로우 자동화가 대폭 강화되었습니다.

2. [Open AI GPT-5.6 on Azure Databricks 정식 지원](https://azure.microsoft.com/updates?id=567431)  
GPT-5.6을 Databricks 내 안전하게 활용할 수 있어, 통합 AI 애플리케이션과 데이터 플랫폼 연동이 더욱 진화했습니다.

3. [Azure Databricks SQL Serverless in UK West 정식 지원](https://azure.microsoft.com/updates?id=567444)  
UK West 리전에서 서버리스 SQL 워크로드 지원으로, 개발·운영자가 인프라 관리에 신경 쓰지 않고 자동 확장형 분석 환경을 구축할 수 있습니다.

4. [Azure AI Language Document PII NextGen Playground 정식 지원](https://azure.microsoft.com/updates?id=564382)  
문서 기반 PII 탐지 기능이 강화되어, 법률·컴플라이언스 팀이 신속하게 민감 정보 검출 및 프로젝트 범위 설정이 가능합니다.

5. [Microsoft Defender security assessments for Azure Database for PostgreSQL Flexible Server 정식 지원](https://azure.microsoft.com/updates?id=567527)  
Defender CSPM 평가로 PostgreSQL 보안 취약점과 미설정 항목을 자동 인식, 실질적 보안 강화와 규제 대응이 쉬워졌습니다.

데이터와 AI·분석 업데이트는 업계 최고 수준의 모델, 보안·컴플라이언스 강화, 서버리스·자동화 분석 플랫폼 구축에 초점을 맞췄습니다.


---

## 🔒 보안, 컴플라이언스, 네트워크 관리

Azure는 보안 자동화와 네트워크 관리 효율화에 집중하며, 데이터 및 서비스 보호 전방위 강화가 트렌드입니다.

1. [Confidential Computing support for Azure Event Hubs Dedicated 정식 지원](https://azure.microsoft.com/updates?id=567212)  
실시간 스트리밍 데이터의 메모리 보호와 하드웨어 기반 TEE로 민감 데이터 처리 시 강력한 보안 제공.

2. [Client-side data integrity protections in Azure Blob Storage 정식 지원](https://azure.microsoft.com/updates?id=566895)  
CRC64-NVME 기반 무결성 검증으로, SDK 단에서부터 저장소까지 데이터의 완전함을 보장합니다.

3. [HTTP header insertion in Azure Firewall 정식 지원](https://azure.microsoft.com/updates?id=568115)  
파이어월에서 HTTP 헤더를 직접 삽입, 테넌트 제한, SaaS 접근 제어 등 보안·업무 시나리오 구현이 단순화되었습니다.

4. [Network Security Perimeter support for Azure Event Hubs 정식 지원](https://azure.microsoft.com/updates?id=567203)  
PaaS 리소스의 네트워크 경계 설정 지원으로, 데이터 유출 위험 감소와 퍼블릭 접근 통제기능이 강화되었습니다.

5. [Symmetric keys on Azure Key Vault Premium 미리 보기](https://azure.microsoft.com/updates?id=566746)  
AES 기반 대칭키 관리와 CNSA 2.0 요구사항 대응으로, 키 Vault의 중앙화된 보안 관리 기능이 한 단계 업그레이드됩니다.

이번 달 보안·컴플라이언스 업데이트는 클라우드 보호 체계의 자동화, 실무적 적용성 확대를 크게 강화한 것이 특징입니다.


---

## 💾 스토리지, 데이터 이동 및 운영 효율화

클라우드 데이터의 이동, 저장, 관리 효율성을 높인 실질적 기능 개선이 이어졌습니다.

1. [Microsoft Entra ID-based access for Azure Blob Storage SFTP 정식 지원](https://azure.microsoft.com/updates?id=567085)  
Entra ID 기반 인증으로 SFTP 접근시 보안 강화, 외부 협업자 onboarding 자동화 및 운영 부하 감소.

2. [Azure Storage Mover migration from Google Cloud Storage (GCS) 미리 보기](https://azure.microsoft.com/updates?id=566948)  
GCS 데이터를 Azure Blob에 마이그레이션할 수 있어 멀티클라우드 통합의 효율과 보안이 크게 향상되었습니다.

3. [Encryption in Transit for Azure Files NFS in AKS 정식 지원](https://azure.microsoft.com/updates?id=567787)  
NFS v4.1 볼륨과 AKS 워크로드 간 데이터 암호화로 컴플라이언스 및 보안 요구 대응이 쉬워짐.

4. [Azure NetApp Files SMB Oplock 설정 지원 미리 보기](https://azure.microsoft.com/updates?id=568396)  
SMB 파일 볼륨의 캐싱 최적화와 데이터 통신 효율화, 운영 환경 안정성 확보.

5. [Instant Access via application consistent restore points 미리 보기](https://azure.microsoft.com/updates?id=565758)  
VM 복구 시 복원 지점 생성 즉시 디스크를 사용할 수 있어, 복구 작업의 신속성과 일관성이 대폭 개선되었습니다.

이번 달 스토리지 부문의 강화는 멀티클라우드 전략, 보안/복구 자동화와 성능 최적화가 중심입니다.


---

## ⚙️ 관리, 거버넌스, DevOps 및 운영 자동화

운영 효율성과 자동화·관리 능력 강화가 지속적으로 추진되었습니다.

1. [Azure Automation supports PowerShell 7.6 runbooks 정식 지원](https://azure.microsoft.com/updates?id=568102)  
최신 파워셸 런북과 런타임 환경 업그레이드, CLI 명령 지원 및 코드 관리 효율성 증대.

2. [Azure Chaos Studio Workspaces & Scenarios 미리 보기](https://azure.microsoft.com/updates?id=567184)  
어플리케이션 중심의 장애 테스트(시나리오)와 자동 리소스 탐색을 통한 운영 리스크 관리가 혁신적으로 진화.

3. [Azure Monitor Logs mirroring into Microsoft Fabric 미리 보기](https://azure.microsoft.com/updates?id=568322)  
Azure Monitor 텔레메트리를 Microsoft Fabric에서 실시간 분석, 비즈니스 데이터와 연계 가능한 통찰력 제고.

4. [Export historical data from Log Analytics workspace with Export jobs 미리 보기](https://azure.microsoft.com/updates?id=566591)  
로그 Analytics 데이터의 특정 기간/쿼리별 추출 및 외부 저장, 규제 대응부터 AI·ML 모델 학습까지 지원.

5. [Support 5x churn in Azure Site Recovery 정식 지원](https://azure.microsoft.com/updates?id=566966)  
VM 당 최대 500MB/s(5배) 처리량으로 고성능 워크로드의 재해복구 신뢰성이 크게 향상되었습니다.

운영 자동화 및 관리의 혁신은 ‘자동화-관찰성-리스크 대응’의 통합 플랫폼 실현을 주도했습니다.


---

## 🧰 Microsoft Foundry & 📊 Microsoft Fabric

Microsoft Foundry와 Fabric은 AI·데이터 혁신의 실무 적용을 한 단계 끌어올렸습니다.

### Microsoft Foundry

1. [Toolboxes in Microsoft Foundry 정식 지원](https://azure.microsoft.com/updates?id=563481)  
조직 내 AI 툴킷의 통합·재사용이 가능, 에이전트 팀 간 상호운용성과 거버넌스 확보가 확대되었습니다.

2. [Document PII playground sample in Microsoft Foundry NextGen 미리 보기](https://azure.microsoft.com/updates?id=563331)  
문서 기반 PII 탐지 Playground 도입, 실시간 샘플 활용으로 API 적용 전 신속한 평가 가능.

3. [Protect sensitive generative AI telemetry in Application Insights and Foundry 미리 보기](https://azure.microsoft.com/updates?id=567594)  
AI 텔레메트리(프롬프트, 응답 등)의 보호 기능 확장, 민감 데이터 접근 제어가 한층 강화되었습니다.

4. [Document PII NextGen Playground in Azure AI Language 정식 지원](https://azure.microsoft.com/updates?id=564382)  
PII 탐지의 신속한 샘플링 및 실무 적용, 컴플라이언스 작업 시나리오 지원.

5. [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)  
(Foundry 연동 가능) 최신 파워셸 런타임 미리 보기 지원, 에이전트·자동화의 최신화 지원.

### Microsoft Fabric

1. [Azure Monitor Logs mirroring into Microsoft Fabric 미리 보기](https://azure.microsoft.com/updates?id=568322)  
Azure Monitor Log Analytics 데이터를 Fabric OneLake으로 실시간 연동, 비즈니스 및 운영 데이터 통합 분석이 가능해졌습니다.

데이터·AI 플랫폼 확장, 민감 정보 보호 자동화, 실무 적용성 확보가 주요 테마입니다.


---

## 🌏 신규 리전, 글로벌 확장, 지역별 업데이트

글로벌 인프라 확장과 지역별 최적화가 더욱 활발히 진행되었습니다.

1. [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)  
인도 Hyderabad에 Azure South Central 리전 개설, AI 준비된 인프라, 데이터 레지던시 강화, 지역 서비스 최적화.

2. [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)  
포스트그레SQL Flexible Server를 인도 South Central 리전에서 정식 지원, 애플리케이션 데이터 분산의 지역 최적화 지원.

3. [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)  
칠레 최초의 Azure 리전 개설 및 ARO 정식 지원, 데이터 레지던시/규제 대응을 갖춘 클라우드 네이티브 환경 구축.

4. [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)  
UK West 내 서버리스 분석 환경 확장.

5. [Document PII Playground 등 글로벌 Foundry 업데이트](https://azure.microsoft.com/updates?id=564382)  
지역별 대규모 엔터프라이즈 적용을 위한 데이터 보호 환경 강화.

리전 개설, 서비스의 글로벌 확장, 지역 거버넌스·레지던시 준수 등 글로벌 기반이 급속하게 확장되었습니다.


---

## ⏳ 사용 중단 및 기타 주요 공지

서비스와 런타임의 사용 중단, 운영 정책 변경 등도 상세히 안내되었습니다.

1. [Support for Python-2.7; 3.8 and PowerShell-7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)  
Automation에서 Python 2.7, 3.8, PowerShell 7.1, 7.2 지원 종료 예정. 보안 업데이트 및 기술 지원은 더 이상 제공되지 않으니 최신 버전으로 업그레이드 필요.

2. [Reservation exchanges for Azure services supported by savings plans will no longer be available starting February 1, 2027](https://azure.microsoft.com/updates?id=568514)  
2027년 2월 1일부터 일부 서비스(Compute, Database 등) Savings Plan이 적용된 예약 교환 정책이 종료되며, 기존 예약은 한 번의 최종 교환만 가능합니다.

3. [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)  
최신 PowerShell 런타임 미리보기 도입과 함께 기존 런타임 사용 중단을 대비하도록 안내.

4. [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)  
기존 PowerShell 모듈 교체 및 신규 기능 지원 등 실무 환경의 표준화 및 최신화 안내.

5. [Azure Chaos Studio Workspaces and Scenarios](https://azure.microsoft.com/updates?id=567184)  
강화된 Chaos Studio 기능 활용과 함께, 기존 아키텍처의 표준화·최신화가 권장되었습니다.

이번 달 주요 공지와 사용 중단 안내는 변화하는 클라우드 환경에 대한 적극적 대처, 업그레이드 필요성을 강조하고 있습니다.


---

## 총평 및 다음 달 전망

2026년 7월 Azure 업데이트는 전방위적 혁신과 플랫폼 신뢰성 강화의 결정판입니다. AI·머신러닝, 보안, 자동화, 데이터 관리, 인프라 확장 등 클라우드 핵심 영역에서 정식 지원(GA)과 미리 보기(Preview)를 포함한 다양한 기능 개선이 실무적 적용성과 확장성을 동시에 추구했습니다.  
특히 Microsoft Foundry와 Azure Databricks, Microsoft Fabric 등 데이터·AI 플랫폼의 실질적 연동성과 조직 전체 적용의 편의성이 한층 강화되었습니다.  
보안·컴플라이언스 자동화, 멀티클라우드·네트워크 현대화, 자동화 관리 도구의 통합도 두드러집니다.

다음 달에는 Azure의 기능별 통합, AI 업무 적용 확대, 하이브리드 환경 자동화, 글로벌 리전 확장, 서비스별 마이그레이션 지원 지속, 그리고 최신 런타임/플랫폼 업그레이드의 본격적인 실무 확대가 전망됩니다. 사용 중단 및 정책 변경도 함께 수시로 확인하여, 변화하는 Azure 생태계에 유연하게 대응해야 할 시기입니다.