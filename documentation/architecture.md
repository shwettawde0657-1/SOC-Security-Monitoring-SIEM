# SOC Architecture

## Architecture

```text
┌──────────────────────┐
│   Windows Machine    │
│                      │
│ Windows Event Logs   │
└──────────┬───────────┘
           │
           │ Security Events
           ▼
┌──────────────────────┐
│    Elastic Agent     │
│    Log Collection    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│    Elasticsearch     │
│     Log Storage      │
└──────────┬───────────┘
           │
           ▼
┌────────────────────────────┐
│       Kibana SIEM          │
│                            │
│  ├── Discover              │
│  ├── Security Dashboard    │
│  ├── Detection Rules       │
│  └── Alerts                │
└────────────┬───────────────┘
             │
             ▼
┌──────────────────────┐
│   SOC Investigation  │
└──────────────────────┘
