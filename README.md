# RFP
Request For proposal  Idea sample

```
flowchart LR
    subgraph Client
        A[User / Admin Web App<br>(React.js + Tailwind)]
        B[Driver Mobile App<br>(React Native)]
    end

    subgraph Backend
        C[Express.js API<br>(Node.js)]
        D[(MongoDB Database)]
    end

    subgraph Cloud
        E[AWS EC2<br>App Hosting]
        F[AWS S3<br>Storage / Media]
        G[Route53<br>Domain + DNS]
    end

    subgraph External_APIs
        H[Google Maps API]
        I[Firebase Cloud Messaging]
    end

    A <--> C
    B <--> C
    C <--> D
    C --> E
    E --> F
    E --> G
    C --> H
    C --> I

    classDef main fill:#e0f7fa,stroke:#006064,stroke-width:1px,color:#004d40,font-weight:bold;
    class A,B,C,D,E,F,G,H,I main;



```
