# FPGA_1GE_Card
This is a Gigabit Ethernet transceiver with GPIO interface. It provides network data transfer at up to 1 Gbps with the host board via 3.3V GPIO. In addition, it is a fully integrated Ethernet solution that enables rapid project implementation, reducing development time and allowing you to focus on the core functions of the system.

## Структура директории

```
.
├── AD
│   ├── board.PcbDoc
│   ├── Capacitors.SchLib
│   ├── Capacitors SMD.PcbLib
│   ├── Capacitors THD.PcbLib
│   ├── Connectors.PcbLib
│   ├── Connectors.SchLib
│   ├── Crystals and Oscillators.PcbLib
│   ├── Crystals & Oscillators.SchLib
│   ├── dev_board_top.SchDoc
│   ├── ethernet.SchDoc
│   ├── fpga_1ge_card.PrjPcb
│   ├── fpga_1ge_card.PrjPcbStructure
│   ├── Inductor and Transformers.PcbLib
│   ├── Inductors & Transformers.SchLib
│   ├── Logic.PcbLib
│   ├── Logic.SchLib
│   ├── power.SchDoc
│   ├── Power Supplies.PcbLib
│   ├── Power Supplies.SchLib
│   ├── Resistors.SchLib
│   ├── Resistors SMD.PcbLib
│   └── Resistors THD.PcbLib
└── README.md
```

## Описание файлов проекта

**fpga_1ge_card.PrjPcb** - файл верхнего уровня для проекта  

**dev_board_top.SchDoc** - принципиальная электрическая схема для всего проекта. Объединяет в себе
**ethernet.SchDoc** и **power.SchDoc**.  
**ethernet.SchDoc** - принципиальная электрическая схема для ethernet-контроллера  
**power.SchDoc** - принципиальная электрическая схема питания для микросхем ethernet.  

**board.PcbDoc** - печатная плата  

## Описание библиотек SchLib

**Capacitors.SchLib** - библиотека условных графических обозначений для конденсаторов  
**Connectors.SchLib** - библиотека условных графических обозначений для коннекторов  
**Crystals & Oscillators.SchLib** - библиотека условных графических обозначений для кварцевых генераторов и резонаторов  
**Inductors & Transformers.SchLib** - библиотека условных графических обозначений для индуктивностей и трансформаторов  
**Logic.SchLib** - библиотека условных графических обозначений для цифровых микрух, по типу процессоров, плисок и т.д.  
**Power Supplies.SchLib** - библиотека условных графических обозначений для источников питания (как для цельных, так и для отдельных микросхем реализующих шим и т.д.)  
**Resistors.SchLib** - библиотека условных графических обозначений для резисторов  

## Описание библиотек PCBLib

**Capacitors SMD** - библиотека посадочных мест для smd конденсаторов  
**Capacitors THD** - библиотека посадочных мест для выводных конденсаторов  
**Connectors** - библиотека посадочных мест для коннекторов (штырьки, пады и т.д.)  
**Crystals and Oscillators** - библиотека посадочных мест для кварцевых генераторов и резонаторов  
**Inductor and Transformers** - библиотека посадочных мест для индуктивностей и трансформаторов  
**Logic** - библиотека посадочных мест для цифровых микрух, по типу процессоров, плисок и т.д.  
**Power Supplies** - библиотека посадочных мест для источников питания (как для цельных, так и для отдельных микросхем реализующих шим и т.д.)  
**Resistors SMD** - библиотека посадочных мест для smd резисторов  
**Resistors THD** - библиотека посадочных мест для выводных конденсаторов  


## Статус разработки

| Файл                            | Разработчик                                 | Статус | Кому/что необходимо доделать? |
|---------------------------------|---------------------------------------------|:------:|-------------------------------|
| Capacitors.SchLib               | Nikilo13, V-Digitronics                     |   ❌   | V-Digitronics: подключить посадочное место к компоненту |
| Connectors.SchLib               | Nikilo13, V-Digitronics, saziliya2003-rgb   |   ✅   | V-Digitronics: перерисовать разъем RJ-45; MrDoomsday: подключить посадочные места для внешних разъемов |
| Crystals & Oscillators.SchLib   | saziliya2003-rgb                            |   ❌   | saziliya2003-rgb: подключить посадочное место к компоненту |
| Inductors & Transformers.SchLib | Nikilo13                                    |   ❌   | Nikilo13: подключить посадочное место к компоненту |
| Logic.SchLib                    | Nikilo13                                    |   ✅   | - |
| Power Supplies.SchLib           | Nikilo13, saziliya2003-rgb                  |   ❌   | saziliya2003-rgb: подключить посадочное место к компоненту |
| Resistors.SchLib                | Nikilo13                                    |   ✅   | - |
| Capacitors SMD.PcbLib           | Nikilo13, V-Digitronics                     |   ✅   | V-Digitronics: сделать посадочное место под электролит  |
| Capacitors THD.PcbLib           | -                                           |   ✅   | - |
| Connectors.PcbLib               | MrDoomsday                                  |   ❌   | MrDoomsday: сделать посадочные места для внешних разъемов  |
| Crystals and Oscillators.PcbLib | saziliya2003-rgb                            |   ❌   | saziliya2003-rgb: сделать посадочное место под генератор |
| Inductor and Transformers.PcbLib| Nikilo13                                    |   ❌   | Nikilo13: сделать посадочное место под катушку |
| Logic.PcbLib                    | Nikilo13                                    |   ✅   | - |
| Power Supplies.PcbLib           | saziliya2003-rgb                            |   ❌   | Nikilo13: сделать посадочное под микр. питания |
| Resistors SMD.PcbLib            | Nikilo13                                    |   ✅   | - |
| Resistors THD.PcbLib            | -                                           |   ✅   | - |
|                                 |                                             |        |   |
| dev_board_top.SchDoc            | -                                           |   ❌   | - |
| ethernet.SchDoc                 | V-Digitronics                               |   ❌   | - |
| power.SchDoc                    | saziliya2003-rgb                            |   ❌   | - |
| board.PcbDoc                    | Nikilo13, V-Digitronics, saziliya2003-rgb   |   ❌   | - |
