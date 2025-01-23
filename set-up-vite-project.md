# Start vite-project with pnpm
1. Check Node.js version by typing `node -v` in the terminal. Update if necassary.
2. Create repository (on github) and clone the remote repository to your computer.
3. Install vite (with TypeScript, no framework for this)
   - `pnpm create vite .`
   - Follow the prompts
   - `pnpm install`
4. Create or update .gitignore file
5. Create vite.config.ts and add following:
```
import { defineConfig } from 'vite';

export default defineConfig({
  'base': '/adress-to-your-repo-here/' // TODO: Change to your repo-name
});
```
6. Install ESLint
  - `pnpm add -D eslint`
  - `pnpm create @eslint/config@latest`
  - Answer questions
7. Install Prettier
  - `pnpm add -D --save exact-prettier`
  - `node --eval "fs.writeFileSync('.prettierrc','{}\n')"`
  - `node --eval "fs.writeFileSync('.prettierignore','# Ignore artifacts:\nbuild\ncoverage\n')"`
  - `pnpm install -D eslint-config-prettier`
  - Add rules to .prettierrc
8. Install Sass
  - `pnpm add sass -D`
  - import sass-file in main.ts
  - `import 'style.scss';`
