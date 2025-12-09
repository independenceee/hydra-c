graph TD
    subgraph L1Block ["LAYER-1 (Cardano Main Chain)"]
        Main[LAYER-1<br/>Chỉ ghi kết quả cuối]
        style Main fill:#e91e63,color:white,font-size:16px
    end

    subgraph Hydra ["HYDRA — Hàng nghìn làn riêng"]
        H1[Head #1<br/>10k+ TPS]
        H2[Head #2<br/>10k+ TPS]
        H3[Head #3<br/>10k+ TPS]
        Hn[Head #n<br/>...]
        style H1,H2,H3,Hn fill:#00c853,color:black
    end

    User[Người dùng<br/>DeFi • Game • Payment] --> H1
    User --> H2
    User --> H3
    User --> Hn

    H1 -->|snapshot cuối| Main
    H2 -->|snapshot cuối| Main
    H3 -->|snapshot cuối| Main
    Hn -->|snapshot cuối| Main
