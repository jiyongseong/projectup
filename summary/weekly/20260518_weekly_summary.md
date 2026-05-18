# Azure 주간 업데이트 요약 - 2026년 05월 18일

## 🗃️ 스토리지 및 데이터 서비스

지난주에는 주요 스토리지 서비스의 문법, 보안, 대규모 파일 처리 등에서 굵직한 변화가 있었습니다. Rust 개발자를 위한 Blob Storage SDK 공식 출시로 현대적 언어 통합이 강화되었고, Azure Files에 관리형 ID 기반 SMB 접근이 정식 지원되면서 비밀키 없는 파일 접근 및 권한 관리를 손쉽게 할 수 있게 되었습니다. 또한, Azure NetApp Files은 볼륨 당 최대 64TiB 대용량 파일 지원을 통해 대규모 온프레미스 워크로드의 클라우드 전환을 간소화합니다. 이처럼 스토리지 영역 변화는 데이터 인프라의 보안, 민첩성, 거버넌스, 확장성 면에서 큰 변혁을 예고합니다.

### [Azure Blob Storage SDK for Rust 정식 지원](https://azure.microsoft.com/updates?id=562516)
Rust 개발 환경에서 Blob 컨테이너 및 객체 업로드·다운로드 등 주요 기능을 정식으로 사용할 수 있게 되었으며, Entra ID 인증, 오류 자동 재시도, 분산 추적까지 지원합니다.

### [Azure Files SMB 관리형 ID 지원 정식 출시](https://azure.microsoft.com/updates?id=562350)
서비스 프린시플 키 없이 Entra 토큰과 RBAC를 활용한 안전한 파일 공유, 키 관리 자동화, 중앙 정책 적용 등 보안성과 운영성이 크게 향상됐습니다.

### [Azure NetApp Files 최대 64TiB 볼륨 제공](https://azure.microsoft.com/updates?id=561722)
모든 Azure NetApp Files 지원 리전에서 대용량 VM 디스크 및 데이터 집합을 무중단 이관하고 클라우드에서 고성능 대용량 파일 워크로드 운영이 가능합니다.

---

## 🔐 보안 및 네트워킹

보안 및 네트워크 분야는 방화벽/네트워크 정책의 사전 검증 및 관리 효율성, 위협 인텔리전스 처리 정확성, 데이터 사용 중 보호 강화에 집중된 업데이트가 이루어졌습니다. Azure Virtual Network Manager의 규칙 영향 분석 기능이 정식 도입되어 네트워크 정책 적용 전 영향 시뮬레이션이 가능해졌고, Sentinel TI는 패턴 파싱에 AND 연산 추가와 신뢰성 향상으로 정확한 위협 식별이 용이해졌습니다. Service Bus Premium의 Confidential Computing 지원은 데이터 보호 범위를 사용 중 데이터까지 확장, 클라우드 보안 수준을 크게 높였다는 점이 특징입니다.

### [Azure Virtual Network Manager 규칙 영향 분석 공식 지원](https://azure.microsoft.com/updates?id=562010)
가상 네트워크 정책의 실제 적용 전 효과를 시뮬레이션하고 운영 중 트래픽 흐름에 미치는 영향을 사전에 파악할 수 있습니다.

### [Sentinel TI 패턴 파싱 AND 연산 지원 및 Revoke 신뢰도 개선](https://azure.microsoft.com/updates?id=561510)
복합 조건 기반 위협 식별, 패턴 관리의 자동화, 일관된 정책 적용이 대폭 강화돼 보안 인시던트 대응력이 향상됩니다.

### [Service Bus Premium 기밀 컴퓨팅 정식 지원](https://azure.microsoft.com/updates?id=561942)
TEE(신뢰 실행 환경) 기반 메시지 처리로 데이터 사용 단계까지 무단 접근을 차단, 하드웨어 수준 보안성을 제공합니다.

---

## 💡 서비스 통합 및 메시징

서비스 통합 분야에서는 Service Bus Premium의 신뢰성과 보안이 대폭 강화되어, 엔터프라이즈 메시징 워크로드의 운영 안정성과 데이터 보호 수준이 업계 최고 수준으로 도약했습니다. 주요 개선점은 가용성 영역(AZ) 기반 리전 전체에 적용되는 99.99% SLA 일괄 확대와 Confidential Computing의 정식 지원이며, SLA 정책 변화 및 세부 세팅이 안내되었습니다. 이를 통해 중요한 금융·공공 워크로드의 Azure 메시징 서비스 채택이 늘어날 것으로 전망됩니다.

### [Service Bus Premium - AZ 지원 리전 99.99% 가동 SLA](https://azure.microsoft.com/updates?id=561947)
모든 AZ 제공 리전의 Service Bus Premium 네임스페이스가 99.99% 간편 SLA에 포함되어 미션 크리티컬 워크로드 신뢰성이 확보됩니다.

### [Service Bus Premium Confidential Computing 정식 지원](https://azure.microsoft.com/updates?id=561942)
TEE 기술로 메시지 전송 및 처리 단계에서 데이터 보호가 극대화되어 민감 정보 처리 환경에서 서비스 활용도가 높아집니다.

### [SLA 정책 및 상세 내용 안내](https://azure.microsoft.com/updates?id=561947)
SLA 정책·인증 기준과 변경 안내, 관련 문서·블로그에서 상세 가이드를 제공하고 있어 운영 및 기획 부서의 참고가 용이합니다.

---

## 🧪 개발 및 클라우드 네이티브

클라우드 네이티브 개발을 위한 도구 및 서비스가 한층 진화했습니다. Rust용 Blob Storage API의 안정화와 Azure Container Apps Express의 퍼블릭 미리 보기 오픈을 통해, 빠르고 자동화된 앱 배포와 운영이 가능해졌습니다. 특히 관리형 ID/비밀 관리, 자동 스케일링 등 현대적 개발 요구사항을 기본 제공하며, Azure Files의 키리스 SMB 인증이 AKS 등 클라우드 네이티브 워크로드의 보안 및 운영 효율을 혁신적으로 개선하고 있습니다.

### [Azure Blob Storage SDK for Rust 정식 지원](https://azure.microsoft.com/updates?id=562516)
효율적인 Rust 애플리케이션 개발과 운영을 위한 공식 스토리지 연동 기능 제공, 생산성 및 안정성이 높아졌습니다.

### [Azure Container Apps Express 퍼블릭 미리 보기 출시](https://azure.microsoft.com/updates?id=559242)
별도의 인프라 셋업 없이 초고속 앱 배포, 자동 스케일링, 통합 관리 환경을 경험할 수 있는 최신 플랫폼입니다.

### [Azure Files 관리형 ID 기반 SMB 접근 지원](https://azure.microsoft.com/updates?id=562350)
CI/CD 파이프라인, AKS 등 클라우드 네이티브 환경에 최적화된 안전하고 효율적인 파일 공유 방식이 적용되었습니다.

---

## 🏭 Microsoft Foundry

Microsoft Foundry 플랫폼은 RBAC 체계가 대폭 개선되어, 역할별 권한 분리 및 할당·위임 자동화가 가능해졌습니다. 기존 Azure AI Role이 브랜드 정체성에 맞춰 Foundry Role로 통합되며, 계정 소유자와 관리자가 로그 분석, 컨테이너 레지스트리 등 종속 역할을 간편하게 할당할 수 있게 되었습니다. 이는 AI/ML 프로젝트 보안성, 워크플로의 유연성 및 대규모 프로젝트에서의 운영 효율을 한단계 높여줍니다.

### [Microsoft Foundry 내장 RBAC 역할 체계 개편](https://azure.microsoft.com/updates?id=562533)
Foundry 계정 및 프로젝트 관리 역할이 명확히 구분되고, 대리 권한 할당·위임 기능이 대폭 강화되었습니다.

### [Foundry RBAC 개념과 상세 구성 문서](https://learn.microsoft.com/en-us/azure/foundry/concepts/rbac-foundry?tabs=owner)
RBAC 모델의 실제 구성, 종속 역할 할당, 활용 예시 등 보안·운영 가이드가 상세히 제공됩니다.

### [Foundry 계정 소유자·관리자 권한 확대](https://azure.microsoft.com/updates?id=562533)
계정 소유/관리자들이 로그, 데이터 관리자 등 핵심 운영 권한을 유연하게 위임할 수 있어, 프로젝트별 보안 요구에 효과적으로 대응할 수 있습니다.

---

## 🇰🇷 한국 리전 주요 업데이트

한국 지역(Korea Central)에서 Azure Service Bus Premium의 Confidential Computing이 정식으로 지원되면서, 데이터 사용 단계의 하드웨어 보안이 한층 강화되었습니다. 금융, 공공 등 고도의 데이터 보안이 필수적인 업종에서 Azure Service Bus 채택이 더욱 증가할 것으로 예상됩니다. 실제 활용 사례와 보안 정책, 적용 사례 등 실무 참고 자료도 다수 제공되고 있어 한국 리전 현업 담당자의 활용도가 높아질 전망입니다.

### [한국 중앙 리전 – Service Bus Premium Confidential Computing 정식 지원](https://azure.microsoft.com/updates?id=561942)
한국 리전에서 기밀 컴퓨팅 활성화로 인-유즈 데이터 보호와 무단 접근 방지가 가능해졌습니다.

### [블로그: Service Bus Confidential Computing GA](https://techcommunity.microsoft.com/blog/messagingonazureblog/announcing-general-availability-of-confidential-computing-for-azure-service-bus-/4517931)
한국 리전에서의 활용 사례, 보안 적용 효과 분석 등 심층 정보를 공식 블로그에서 확인할 수 있습니다.

### [문서: Service Bus Confidential Computing](https://learn.microsoft.com/azure/service-bus-messaging/confidential-computing)
한국 리전별 적용 정책, 구축 가이드, 실착용 케이스 등 실무 중심의 참고자료가 제공됩니다.