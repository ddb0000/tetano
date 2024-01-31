# project structure

.tetano/
│
├── Cargo.toml              # Dependency manifest
├── Cargo.lock              # Dependency lock file (auto-generated)
│
├── src/
│   ├── lib.rs              # Library root (contains framework core logic)
│   ├── server.rs           # Server setup and request handling
│   ├── router.rs           # Routing logic
│   ├── middleware.rs       # Middleware implementation
│   ├── handler.rs          # Request handlers
│   ├── response.rs         # Response structures and utilities
│   ├── request.rs          # Request parsing and utilities
│   ├── constants.rs        # Constants used across the framework
│   └── utils/              # Utility functions and helpers
│       ├── mod.rs          # Makes utils a module
│       └── ...             # Other utility modules (e.g., error handling, logging)
│
├── examples/               # Example applications using Tetano
│   ├── basic/
│   │   ├── main.rs         # A basic example
│   │   └── Cargo.toml      # Dependency manifest for the example
│   └── ...                 # More complex examples (e.g., file upload, database interaction)
│
├── tests/                  # Integration and unit tests
│   ├── integration.rs      # Integration tests
│   └── ...                 # Other test files (e.g., unit tests for each module)
│
├── benchmarks/             # Performance benchmarks
│   ├── throughput.rs       # Throughput benchmarks
│   └── ...                 # Other benchmarks (e.g., latency, memory usage)
│
└── docs/                   # Documentation sources
    ├── getting_started.md  # Getting started guide
    └── ...                 # Detailed documentation for each module, FAQ
