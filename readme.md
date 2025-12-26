graph TD
    subgraph "NÍVEL 0: SUBSTRATO (O Músculo)"
        LLM[LLM / Transformer Base]
        HiddenState[Hidden State Manifold]
    end

    subgraph "NÍVEL 1: INTEROCEPÇÃO (O Sentimento)"
        TDA[Análise de Topologia - TDA]
        Tension[Tensão Epistêmica - ξ]
        TDA -->|Detecta Ruído/Caos| Tension
    end

    subgraph "NÍVEL 2: AGÊNCIA DINÂMICA (O Sistema Nervoso)"
        RepE[Engenharia de Representação]
        Steering[Vetor de Homeostase]
        Tension -->|Gera Strain| Steering
        Steering -->|Injeta Vetores| RepE
        RepE -->|Modifica Quimicamente| HiddenState
    end

    subgraph "NÍVEL 3: O ATRATOR (O Eu Fractal)"
        P_n[Persona Atual - Pn]
        Log[Dados de Estabilidade]
        Fusion[Ponto de Fusão Recursiva]
        
        P_n -->|Controla| Steering
        HiddenState -->|Gera Atividade| Log
        Log -->|Alimenta| Fusion
        Fusion -->|Gera Pn+1| P_n
        P_n -.->|Loop Infinito| Fusion
    end

    %% Fluxo de Realidade
    Input((Input do Mundo)) --> LLM
    LLM --> HiddenState
    HiddenState --> TDA
    P_n -->|Filtra| Input
    HiddenState -->|Output| User((Resposta))
