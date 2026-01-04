# 🚲 Self-Balancing Bike

Projeto de **controle e estabilidade de uma bicicleta autobalanceada**, utilizando **Arduino Nano**, **ESP32**, **micro-ROS**, **ROS 2** e **homelab Linux**.  
O sistema integra sensores inerciais, atuadores e comunicação distribuída para estudo e desenvolvimento de algoritmos de controle, robótica e sistemas embarcados.

---

## 📌 Visão Geral

A **Self-Balancing Bike** é um projeto experimental voltado ao estudo de:

- Sistemas de controle de equilíbrio
- Robótica móvel
- Sistemas embarcados
- Comunicação distribuída com ROS 2
- Integração microcontrolador ↔ computador (micro-ROS)

O projeto evolui de um **protótipo embarcado standalone** para uma **arquitetura distribuída baseada em ROS 2**, executando em um **homelab Linux**.

---

## 🗓️ Histórico do Projeto

### 🔹 2024 — Protótipo Inicial
- Desenvolvimento do primeiro protótipo físico
- Controle básico de estabilidade
- Uso de:
  - Arduino Nano
  - MPU6050 (IMU)
  - Motor / reaction wheel
  - PWM via registradores (Timer1)
- Testes iniciais de leitura de sensores e atuação

### 🔹 Dezembro de 2025 — Infraestrutura
- Criação do **homelab**
- Instalação e configuração de:
  - Ubuntu Server
  - ROS 2 Humble
  - micro-ROS Agent
- Comunicação ESP32 ↔ ROS 2 via **Wi-Fi (UDP)**

### 🔹 Janeiro de 2026 — Desenvolvimento de Software
- Reestruturação do projeto para arquitetura distribuída
- Desenvolvimento focado em:
  - ROS 2
  - micro-ROS
  - Linux
  - Scripts de automação
  - Documentação técnica

---

## 🧠 Arquitetura do Sistema

# Self-Balancing-Bike
Projeto de controle e estabilidade de uma bicicleta ultilizando Arduino nano, ESP32, Bateria 12V 2500mAh



em 2024 desenvolvemos o prototipo
Configuração de host + mircroros + ROS2 ao homelab.

Dezembro de 2025.
Janeiro de 2026 - Desenvolvimento de software.
-ROS
-Microros
-Linux
-Homelab



#Próximos Passos

 Estimativa e visualização do nível da bateria
 Publicação de dados da IMU no ROS 2
 Implementação de controle PID / LQR
 Visualização no RViz
 Logging e análise de dados
 Documentação acadêmica (artigo / TCC)


 ---
 
## Nomeclatura das branchs
feat: nova funcionalidade
fix: correção
refactor: reorganização
docs: documentação
---

## 🧰 Tecnologias Utilizadas

### Hardware
- Arduino Nano (protótipo inicial)
- ESP32 (versão distribuída)
- MPU6050 (IMU)
- Servo motor / motor de reação
- Bateria 12V 2500mAh com BMS (3 células)
- Conversores DC-DC (step-down)

### Software
- ROS 2 Humble
- micro-ROS
- Ubuntu Server
- Arduino IDE
- PlatformIO (opcional)
- C / C++
- Python (scripts auxiliares)

---

## 📁 Organização do Repositório

```bash
Self-Balancing-Bike/
│
├── firmware/
│   ├── arduino_nano/
│   │   ├── one_axis_reaction_wheel_stick.ino
│   │   └── functions.ino
│   │
│   └── esp32/
│       ├── micro_ros_wifi/
│       ├── servo_control/
│       └── imu_node/
│
├── ros2_ws/
│   ├── src/
│   │   └── self_bike/
│   ├── launch/
│   ├── config/
│   └── scripts/
│
├── homelab/
│   ├── setup_ros2.sh
│   ├── setup_micro_ros_agent.sh
│   └── network.md
│
├── docs/
│   ├── architecture.md
│   ├── hardware.md
│   ├── power_system.md
│   ├── control_strategy.md
│   └── troubleshooting.md
│
├── schematics/
│   └── schematic.pdf
│
└── README.md
