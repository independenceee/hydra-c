graph TD
    subgraph "Cardano Main Chain (Layer-1)"
        Main[Block hiện tại\nChỉ ghi kết quả cuối]
        style Main fill:#ff6666,color:#fff
    end

    subgraph "Hydra – Hàng nghìn đường cao tốc riêng tư song song"
        H1[Hydra Head #1\n~10 000 TPS]
        H2[Hydra Head #2\n~10 000 TPS]
        H3[Hydra Head #3\n~10 000 TPS]
        H4[...]

    end

    User[Người dùng / DeFi / Game / NFT] -->|99,9% giao dịch| H1
    User -->|99,9% giao dịch| H2
    User -->|99,9% giao dịch| H3
    User -->|99,9% giao dịch| H1000

    H1 -->|Chỉ snapshot cuối| Main
    H2 -->|Chỉ snapshot cuối| Main
    H3 -->|Chỉ snapshot cuối| Main
    H1000 -->|Chỉ snapshot cuối| Main

    style H1 fill:#66ff66
    style H2 fill:#66ff66
    style H3 fill:#66ff66
    style H1000 fill:#66ff66
    note3[Tốc độ Layer-2\nBảo mật & finality Layer-1\nKhông bridge – Không chờ 7 ngày]
    style note3 fill:#222,color:#0f0,font-weight:bold
