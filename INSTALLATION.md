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

## Shadcn UI Setup

Run the Shadcn UI initializer after creating the app:

```bash
npx shadcn@latest init
```

During the CLI setup, configure the `components.json` options like this:

- `Style:` Default
- `Base color:` Slate or Zinc are great defaults for a clean look.
- `Do you want to use CSS variables for colors?` Yes

## After Setup

1. Change into the new project folder:

```bash
cd ai-agency-site
```

2. Install recommended UI and integration packages:

```bash
npm install framer-motion firebase lucide-react cloudinary
```

3. Install useful dev tooling:

```bash
npm install -D prettier eslint-config-prettier eslint-plugin-simple-import-sort eslint-plugin-tailwindcss
```

4. Add common Shadcn UI components:

```bash
npx shadcn@latest add button card input badge
```

5. Start the development server:

```bash
npm run dev
```

6. Open the project in the browser:

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

- Use `prettier` alongside ESLint to keep code formatting consistent.

- Firebase can be used for auth, Firestore, or storage while Cloudinary is great for hosted media assets.

## Shadcn UI Notes

After `npx shadcn@latest init`, add initial components that match your landing page layout. Common first components include:

- `button`
- `card`
- `input`
- `badge`
- `popover`

You can add more UI pieces later with:

```bash
npx shadcn@latest add button card input badge
```

## Recommended Next Steps

- Open `src/app/page.tsx` and start customizing the landing page.
- Review `tailwind.config.ts` and `globals.css` for Tailwind setup.
- Add lint scripts or pre-commit hooks later if needed.
