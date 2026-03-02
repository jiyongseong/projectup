# Azure 주간 업데이트 요약 - 2026-02-02

## 📢 정식 지원 (Launched)
Azure의 정식 지원 업데이트는 새로 출시된 기능과 서비스가 최종 개발 단계를 거쳐 안정적인 클라우드 환경을 제공하며, 사용자 경험을 개선하기 위해 설계되었습니다. 이번 주 주요 업데이트에는 PostgreSQL 소규모 버전 지원, Azure Databricks의 Agent Bricks 지능형 어시스턴트, 그리고 AMD v7 기반의 가상 머신이 포함되었습니다. 이들 기능은 클라우드 사용 시 성능 향상과 안정성 증대에 중점을 둡니다.

### [Azure Database for PostgreSQL 최신 소규모 버전 정식 지원](https://azure.microsoft.com/updates?id=550164)
PostgreSQL의 소규모 버전 업데이트가 정식 지원되며, Azure Database for PostgreSQL – Flexible Server에서 자동으로 업그레이드됩니다. 이를 통해 데이터베이스 성능과 보안을 지속적으로 개선합니다. 

### [Azure Databricks Agent Bricks 지능형 어시스턴트 출시](https://azure.microsoft.com/updates?id=542455)
Azure Databricks 플랫폼에서 AI 에이전트 생성과 관리가 더 쉬워졌습니다. 이 기능은 사전 구축된 구성 요소와 통합된 데이터로 AI를 빠르고 효율적으로 배포할 수 있도록 돕습니다.

### [AMD 기반 Dasv7/Easv7/Fasv7 VM 정식 지원](https://azure.microsoft.com/updates?id=552318)
AMD 기반 VM이 정식 지원되고 있으며, 메모리 최적화 및 CPU 성능 개선을 통해 다양한 사용자 워크로드 요구를 충족시킵니다.

---

## 🚀 미리 보기 (In Preview)
미리 보기로 제공되는 Azure 업데이트는 사용자가 최신 기술을 먼저 체험하도록 설계되어 있으며, 클라우드 운영의 최적화를 지원하는 것이 목표입니다. 이번 주에는 Azure Command Launcher for Java, Intel 기반 VM, OpenShift에서 Azure NetApp Files 지원이 포함되었습니다.

### [Azure Command Launcher for Java 미리 보기 출시](https://azure.microsoft.com/updates?id=543994)
Java 컨테이너 및 VM의 최적화를 위해 새로운 JVM 런처가 출시되었습니다. 사용자는 리소스 효율성과 배포 성능을 개선할 수 있습니다.

### [Intel 기반 Dlsv7/Dsv7/Esv7 VM 미리 보기 출시](https://azure.microsoft.com/updates?id=529407)
최신 Intel Xeon 프로세서를 이용한 VM으로 더욱 강력한 성능과 메모리 용량을 제공합니다. 베타 테스트는 특정 지역에서 시작됩니다.

### [OpenShift에서 Azure NetApp Files 지원 추가](https://azure.microsoft.com/updates?id=550466)
OpenShift 가상화가 Azure NetApp Files를 지원하며, VM 프로비저닝 속도와 확장성을 크게 향상시킬 수 있습니다.

---

## ⏳ 지원 종료 (Retirement)
지원 종료 업데이트는 특정 기능이나 서비스가 더 이상 제공되지 않음을 알리는 공지이며, 사용자는 대체 기술로 전환할 준비를 해야 합니다. 주요 업데이트로는 Python 3.10 지원 종료와 Event Hubs 및 Storage로 데이터 전송 기능 중단이 포함됩니다.

### [Azure Functions의 Python 3.10 지원 종료](https://azure.microsoft.com/updates?id=545771)
Python 3.10에 대한 지원이 종료되며, 사용자는 Python 3.13으로 애플리케이션을 업그레이드해야 합니다. 보안 및 성능 최적화를 위해 권장됩니다.

### [Event Hubs 및 Storage로 데이터 전송 기능 지원 종료](https://azure.microsoft.com/updates?id=551523)
Event Hubs와 Storage로 데이터를 보내는 미리 보기 기능이 중단됩니다. 대체 옵션을 사용하여 데이터 전송을 지속하세요.

---

## 📂 스토리지 (Storage)
스토리지 업데이트는 데이터 관리와 안정성을 개선하기 위한 기능을 제공합니다. 이번 주에는 Azure NetApp Files의 OpenShift 지원이 주목받았습니다.

### [OpenShift 가상화에서 Azure NetApp Files 지원](https://azure.microsoft.com/updates?id=550466)
Azure NetApp Files를 통해 OpenShift에서 더 빠른 가상 머신 프로비저닝과 유연한 스토리지 솔루션을 제공합니다.

---

## 💻 컴퓨팅 (Compute)
컴퓨팅 업데이트는 최적화된 가상 머신 및 컨테이너 서비스를 제공하며 클라우드 기반 성능 개선에 중점을 둡니다. Intel과 AMD 기반 VM과 Python 지원 종료가 주요 변동 사항입니다.

### [Intel 기반 Dlsv7/Dsv7/Esv7 VM 미리 보기 출시](https://azure.microsoft.com/updates?id=529407)
최첨단 Intel Xeon 프로세서로 성능과 확장성을 대폭 증가시킨 VM이 미리보기 상태로 제공됩니다.

### [AMD 기반 Dasv7/Easv7/Fasv7 VM 정식 지원](https://azure.microsoft.com/updates?id=552318)
새로운 AMD 기반 VM은 빠른 CPU 성능과 향상된 메모리 최적화를 제공하여 다양한 워크로드에 적합합니다.

### [Azure Functions의 Python 3.10 지원 종료](https://azure.microsoft.com/updates?id=545771)
Python 3.10에 대한 지원이 종료되며 더 현대적인 버전으로의 전환이 필요합니다.