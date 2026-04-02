# Project Installation

Save the project setup and installation notes here.

## Create Next App

Just run the command without any flags at all:

```bash
npx create-next-app@latest ai-agency-site
```

During the setup wizard, make sure to select these options:

- `Would you like to use ESLint?` Yes
- `Would you like to use Tailwind CSS?` Yes
- `Would you like to use src/ directory?` Yes (Highly recommended for organizing larger projects)
- `Would you like to use App Router? (recommended)` Yes (This gives you Server Actions)
- `Would you like to customize the default import alias (@/*)?` Yes (The default @/* is perfect)

## After Setup

1. Change into the new project folder:

```bash
cd ai-agency-site
```

2. Start the development server:

```bash
npm run dev
```

3. Open the project in the browser at:

```text
http://localhost:3000
```

## Notes

- `create-next-app` installs dependencies automatically by default. If the install step is skipped or interrupted, run:

```bash
npm install
```

- The `src/` directory is recommended for keeping React components, pages, and styles organized.

- App Router gives you access to Server Actions and modern Next.js routing patterns.

- The default alias `@/*` works well for clean absolute imports from the `src/` folder.

## Recommended Next Steps

- Open `src/app/page.tsx` and start customizing the landing page.
- Review `tailwind.config.ts` and `globals.css` for Tailwind setup.
- Add lint scripts or pre-commit hooks later if needed.
