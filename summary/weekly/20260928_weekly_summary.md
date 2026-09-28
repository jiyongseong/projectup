# Azure 주간 업데이트 요약 - 2026년 09월 28일

## 🚀 출시 및 정식 지원

지난주 Azure에서는 신규 서비스와 기능의 정식 지원이 다수 발표되었습니다. Azure Functions는 PowerShell 7.6을 지원하여 최신 스크립트 환경에서 개발 및 배포가 간편해졌으며, Azure Sphere OS의 커널 업그레이드는 장기적 보안과 신뢰성을 확보하는데 큰 역할을 합니다. VM 복구 지점 즉시 접근 기능은 복구 시간을 획기적으로 단축해, 비즈니스 연속성과 인프라 안정성에 중요한 변화가 생겼습니다. 전반적으로 운영 효율성이 높아진 것이 특징이며, 장기 지원 정책과 인프라 복구 자동화 등 실질적인 생산성 제고가 이루어진 점이 돋보입니다.

### [Azure Functions PowerShell 7.6 정식 지원 발표](https://azure.microsoft.com/updates?id=572219)
Azure Functions에서 PowerShell 7.6을 정식 지원하게 되어, 최신 PowerShell 기능으로 앱을 개발하고 기민하게 배포할 수 있습니다.

### [Azure Sphere OS 26.09 정식 출시](https://azure.microsoft.com/updates?id=572579)
Azure Sphere OS의 Linux 커널이 6.1.x로 업그레이드되어 장기적 CIP 플랫폼 지원과 보안, 안정성이 강화되었습니다.

### [VM 복구 지점 즉시 접근 기능 정식 지원](https://azure.microsoft.com/updates?id=572573)
VM 복구 시 스냅샷 생성 직후 디스크 복구가 가능해져 빠른 인프라 재해복구와 업무중단 최소화가 가능합니다.


## 🧪 미리 보기 (Preview)

Azure는 미리 보기 기능을 통해 혁신적인 기술 실험을 적극 지원하고 있습니다. 이번 주에는 클라우드 네이티브 데이터베이스 서비스, AKS 하이브리드 엣지 관리, 그리고 개발 생산성 도구가 미리 보기로 공개되었습니다. Azure HorizonDB의 PostgreSQL 18 지원은 최신 DB 업계 트렌드를 반영하며, AKS Flex Nodes는 확장성과 분산 환경 지원을 강화합니다. VS Code에서 Copilot 기반 Azure 앱 개발 미리 보기는 자동화 및 워크플로우 혁신을 통한 개발자의 생산성 향상이 기대됩니다.

### [Azure HorizonDB PostgreSQL 18 지원 미리 보기](https://azure.microsoft.com/updates?id=573048)
Azure HorizonDB가 PostgreSQL 18을 미리 보기로 지원하며, 대규모 로드 환경에서 최신 기능을 경험할 수 있습니다.

### [AKS Flex Nodes 미리 보기 출시](https://azure.microsoft.com/updates?id=571919)
AKS Flex Nodes는 하이브리드 및 엣지 인프라를 AKS 컨트롤플레인에 연결해, 로컬 실행 환경에 적합한 배포 옵션을 제공합니다.

### [VS Code에서 Azure 앱 구축용 Guided Copilot 경험 미리 보기](https://azure.microsoft.com/updates?id=572214)
VS Code에서 구조화된 Copilot 워크플로우를 통해 Azure 앱 개발 자동화와 생산성이 크게 향상됩니다.


## ⛔ 지원 종료 및 사용 중단

Azure는 지속적으로 구버전 런타임과 서비스를 정리하며 최신 환경으로의 전환을 권장합니다. 이번 주 발표된 지원 종료는 ACS 단독 서비스, .NET 8/9, Node.js 22, PowerShell 7.4 등 주요 언어와 커뮤니케이션 플랫폼에 대한 것입니다. 구버전 사용자는 보안 및 성능 리스크가 커지므로, 마이그레이션 및 업그레이드를 반드시 진행해야 하며, Azure Functions에서 In-process 또는 Linux Consumption 플랜 사용자는 추가적인 전환 조치가 필요합니다.

### [Azure Communication Services(ACS) 단독 서비스 지원 종료 (2028년 9월 30일)](https://azure.microsoft.com/updates?id=557117)
여러 ACS 단독 서비스(이메일, SMS, WhatsApp 등)가 2028년 9월 지원 종료 예정이며, Teams 연동과 최신 SDK 업그레이드가 필요합니다.

### [.NET 8 및 .NET 9 지원 종료 (2026년 11월 10일)](https://azure.microsoft.com/updates?id=572838)
Azure Functions에서 .NET 8/9 지원이 2026년 11월까지로, 곧 .NET 10으로 업그레이드해야 보안과 지원이 유지됩니다.

### [Node.js 22 지원 종료 (2027년 4월 30일)](https://azure.microsoft.com/updates?id=572771)
Azure Functions에서 Node.js 22은 2027년 4월 지원 종료되며, Node.js 24로 업그레이드가 반드시 필요합니다.


## 🔑 런타임/언어 지원 정책 변경

Azure Functions 환경에서 런타임 및 언어 지원 정책 변화가 빠르게 진행되고 있습니다. PowerShell 7.4, .NET 8/9, Node.js 22 등은 곧 지원 종료되며, 보안 패치 및 성능 개선을 위해 최신 버전으로의 전환이 중요합니다. 특히 Isolated worker 모델로의 전환과 Flex Consumption 플랜으로의 마이그레이션이 개발 및 운영 효율성을 높입니다. 이에 따라 개발자 및 운영팀은 업데이트 정책에 따라 플랫폼 전략을 선제적으로 수립해야 합니다.

### [PowerShell 7.4 지원 종료 공지 (2026년 11월 10일)](https://azure.microsoft.com/updates?id=572770)
PowerShell 7.4가 지원 종료되어 7.6으로 업그레이드가 필수이며, Linux Consumption 플랜 사용자는 Flex Consumption 전환 후 업그레이드해야 정상 운영이 가능합니다.

### [.NET 8/9 지원 정책 변화 및 업그레이드 안내](https://azure.microsoft.com/updates?id=572838)
In-process 모델 사용자는 반드시 Isolated worker로 마이그레이션 후 .NET 10으로 업그레이드해야 하며, Linux Consumption 플랜에서도 플랜 업그레이드를 동반해야 합니다.

### [Node.js 22 지원 종료 및 정책 변화](https://azure.microsoft.com/updates?id=572771)
Node.js 22에서 Node.js 24로 업그레이드가 강조되며, 기존 Linux Consumption 플랜은 Flex Consumption으로 전환해야만 정상 업그레이드가 가능합니다.


## 🌐 인프라 & 운영 관리

이번 주 Azure 업데이트에서는 VM 복구 지점 즉시 접근, AKS Flex Nodes, 그리고 Azure Sphere OS 장기 지원 정책 등 인프라 및 운영 효율성 혁신이 이루어졌습니다. VM 복구 지점 즉시 접근 기능은 복구 자동화와 시간 단축에 유리하고, AKS Flex Nodes는 분산 환경과 하이브리드 운영에서 중앙 관리 옵션을 부여합니다. Azure Sphere OS 최신화는 커널 보안 강화와 안정적 장기 운영에 직접적인 영향을 미칩니다. 전반적으로 업무 연속성과 보안, 인프라 관리가 한층 더 강화된 점이 주요 포인트입니다.

### [VM 복구 지점 즉시 접근 기능](https://azure.microsoft.com/updates?id=572573)
스냅샷 생성 즉시 디스크 복구가 가능해져 업무 연속성과 인프라 복구 자동화에 도움이 됩니다.

### [AKS Flex Nodes 인프라 관리 혁신](https://azure.microsoft.com/updates?id=571919)
AKS와 하이브리드/엣지 환경 연계로 인프라 중앙 관리가 용이해졌으며, 분산된 비즈니스 요구에 더욱 탄력적인 대응이 가능합니다.

### [Azure Sphere OS 26.09 운영 체제 최신화](https://azure.microsoft.com/updates?id=572579)
Linux CIP Platform 기반 커널 업그레이드로 장기적 시스템 운영에 안전성과 신뢰성이 강화되었습니다.