---
marp: true
title: Introdução a CPS, AADL e ROS
author: Ana Barbosa, Wenderson Nascimento
keywords: ciberfisico, ros, aadl
theme: barbosa
class: style_a
paginate: true
_paginate: false
footer: 2025 © IFRN CNAT
---

<!-- _class: title -->

# Introdução a CPS, AADL e ROS

Ana Barbosa, Wenderson Nascimento

---

## Cyber-Physical Systems (CPS)

O termo *Sistemas Ciberfísicos* refere-se a sistemas que integram capacidades computacionais e físicas, sendo capazes de interagir com seres humanos de diferentes formas.

As pesquisas voltadas para sistemas ciberfísicos têm como objetivo integrar princípios e conhecimentos das áreas de computação e engenharia para desenvolver uma ciência voltada a sistemas ciberfísicos e tecnologias de suporte relacionadas.

---

<!-- _class: style_b -->

### Indústria e Academia

Atualmente, governos e indústrias vêm investindo em tecnologias de sistemas ciberfísicos de longo prazo. Por exemplo, a União Europeia lançou uma iniciativa tecnológica conjunta entre nações europeias chamada *Advanced Research and Technology for Embedded Intelligence Systems* (ARTEMIS).

---

<!-- _class: style_b -->

Iniciativas semelhantes vêm sendo implementadas em outros países, como Estados Unidos, Japão, China, Coreia do Sul e Alemanha.

Existem diversas oportunidades de pesquisa e desenvolvimento, como:

* Biomedicina e Saúde
* Transporte Aéreo (*NextGen*)
* Energia Renovável e Redes Elétricas Inteligentes
* Internet Industrial das Coisas (IIoT)

---

<!-- _class: style_b -->

### Exemplo de CPS

![w:600px](./img/image1.png)

Robô na agricultura

---

## Architecture Analysis & Design Language (AADL)

A AADL é uma linguagem de modelagem utilizada para modelar e analisar arquiteturas de sistemas ciberfísicos e embarcados.

Ela é eficiente para análises baseadas em modelos e especificações de sistemas embarcados complexos de tempo real. Também suporta a análise e previsão antecipada de qualidades críticas do sistema, como desempenho, escalonabilidade e confiabilidade.

---

<!-- _class: style_b -->

### Abstração de Componentes

Na AADL, um componente é caracterizado por seu nome único, interfaces, propriedades, subcomponentes e interações. As abstrações de componentes são separadas em três categorias:

* Software de Aplicação
* Plataforma de Execução (Hardware)
* Composto

---

### Análise de Arquitetura

A AADL pode ser utilizada para modelar e analisar sistemas em uso, prototipar e integrar novos sistemas. Com essa linguagem, conjuntos de propriedades podem ser declarados, permitindo a inclusão de novas propriedades para outros componentes ou elementos, como portas e conexões.

---

<!-- _class: style_b -->

## Robot Operating System (ROS)

O ROS é uma coleção de bibliotecas e ferramentas robóticas de código aberto voltadas para a construção de softwares para robôs. Ele oferece uma plataforma de desenvolvimento que acompanha o projeto desde a prototipação até a implementação.

---

### Propósito e Utilização

O ROS abstrai a camada de hardware e facilita a configuração de cada parte do robô por meio dos pacotes de seu ecossistema. Dessa forma, permite que o desenvolvedor se concentre em outros aspectos do projeto, como lógica e algoritmos.

---

<!-- _class: style_b -->

## Uso da AADL com ROS

A AADL atua na modelagem e validação da arquitetura do sistema. O ROS é utilizado para implementar e integrar os componentes do sistema.

A ideia central é utilizar a AADL como modelo de alto nível para gerar automaticamente código ROS, acelerando o processo de desenvolvimento.

---

<style scoped>section { font-size: 20px; }</style>

<!-- _class: style_c -->

## Referências

*The Architecture Analysis & Design Language (AADL): An Introduction.* Disponível em: https://apps.dtic.mil/sti/html/tr/ADA455842/

*Presentation of the AADL: Architecture Analysis and Design Language.* Disponível em: https://beru.univ-brest.fr/~singhoff/ENS/UE_VFS/CM/part1_introducing_aadl.pdf

*Cyber-Physical Systems.* Disponível em: https://ieeecss.org/sites/ieeecss/files/2019-07/IoCT-Part3-02CyberphysicalSystems.pdf

*A use case in model-based robot development using AADL and ROS.* Disponível em: https://rose-workshops.github.io/files/rose2018/papers/rose2018_2.pdf

ROS - Robotic Operating System. Disponível em: https://www.ros.org/

*Cyber-Physical Systems: An Overview.* Disponível em: https://www.fortinet.com/resources/cyberglossary/cyber-physical-systems
