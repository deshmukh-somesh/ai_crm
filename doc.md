# AI CRM Backend

catalyst-demo-backend/
├── prisma/
│   ├── schema.prisma
│   └── migrations/
├── src/
│   ├── trpc/           # tRPC router definitions
│   │   ├── router.ts
│   │   ├── context.ts
│   │   └── trpc.ts
│   ├── modules/        # Feature modules
│   │   ├── users/
│   │   │   ├── user.router.ts
│   │   │   ├── user.service.ts
│   │   │   ├── user.schema.ts
│   │   │   └── user.types.ts
│   │   ├── auth/
│   │   │   ├── auth.router.ts
│   │   │   ├── auth.service.ts
│   │   │   └── auth.utils.ts
│   │   └── emails/
│   │       ├── email.router.ts
│   │       ├── email.service.ts
│   │       └── email.types.ts
│   ├── lib/           # Shared utilities
│   │   ├── prisma.ts
│   │   ├── openai.ts
│   │   └── jwt.ts
│   ├── middleware/    # Express middleware
│   │   ├── error.ts
│   │   └── auth.ts
│   └── index.ts      # Entry point
├── .env
├── .env.example
├── .eslintrc.json
├── .prettierrc
├── nodemon.json
├── tsconfig.json
└── package.json


# AI CRM Frontend


ai-crm-frontend/
├── .env.local
├── package.json
├── next.config.js
├── tailwind.config.js
├── postcss.config.js
├── public/
│   ├── images/
│   └── favicon.ico
├── src/
│   ├── app/
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   ├── (auth)/
│   │   │   ├── login/
│   │   │   │   └── page.tsx
│   │   │   └── layout.tsx
│   │   ├── dashboard/
│   │   │   ├── page.tsx
│   │   │   └── layout.tsx
│   │   ├── leads/
│   │   │   ├── page.tsx
│   │   │   └── [id]/
│   │   │       └── page.tsx
│   │   └── settings/
│   │       └── page.tsx
│   ├── components/
│   │   ├── ui/
│   │   │   ├── button.tsx
│   │   │   ├── input.tsx
│   │   │   ├── modal.tsx
│   │   │   └── select.tsx
│   │   ├── dashboard/
│   │   │   ├── progress-tracker.tsx
│   │   │   └── stats-card.tsx
│   │   ├── leads/
│   │   │   ├── lead-table.tsx
│   │   │   ├── email-sequence.tsx
│   │   │   └── upload-modal.tsx
│   │   └── shared/
│   │       ├── navbar.tsx
│   │       ├── sidebar.tsx
│   │       └── loading.tsx
│   ├── lib/
│   │   ├── auth.ts
│   │   ├── api.ts
│   │   └── utils.ts
│   ├── hooks/
│   │   ├── use-auth.ts
│   │   └── use-leads.ts
│   ├── providers/
│   │   └── auth-provider.tsx
│   ├── types/
│   │   ├── lead.ts
│   │   ├── user.ts
│   │   └── email.ts
│   └── styles/
│       └── globals.css