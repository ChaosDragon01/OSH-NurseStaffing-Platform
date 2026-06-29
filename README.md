```text


OSH-NurseStaffing-Platform/
│
├── src/
│   ├── OSHStaffing.WebAPI/             # Controller layer serving JSON data
│   │   ├── Controllers/
│   │   │   ├── StaffingController.cs
│   │   │   └── CoverageController.cs
│   │   ├── Program.cs
│   │   └── appsettings.json
│   │
│   ├── OSHStaffing.Core/               # System entities and allocation rules
│   │   ├── Entities/
│   │   │   ├── Nurse.cs
│   │   │   ├── School.cs
│   │   │   └── CoverageRequest.cs
│   │   └── Algorithms/
│   │       └── CoverageMatcher.cs      # Staff matching logic
│   │
│   ├── OSHStaffing.Infrastructure/     # Entity Framework Core Context
│   │   ├── Data/
│   │   │   ├── StaffingDbContext.cs
│   │   │   └── DbInitializer.cs        # Seed files with mock NYC schools/nurses
│   │   └── Scripts/
│   │       └── SetupDatabase.sql       # Complex reporting Views
│   │
│   └── OSHStaffing.Dashboard/          # Frontend client application UI
│       ├── Pages/
│       └── Components/
│
└── OSH-NurseStaffing-Platform.sln