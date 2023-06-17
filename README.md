This is a simple repo exploring [Vercel AI SDK](https://github.com/vercel-labs/ai). It's meant to share the code from my [YouTube Channel](https://youtu.be/VsyIya5PWb0):

This is by all means not production ready software. This is just to help get you started quickly.

## Getting Started

1. Make sure you register for an OpenAI API key. ([See how to here](https://www.howtogeek.com/885918/how-to-get-an-openai-api-key/))
2. Copy `.env.example` to a new file called `.env` or `.env.local` **`.env` is tracked in git, be careful about handling your API key properly**
3. install dependencies

```bash
npm install
# or
yarn install
# or
pnpm install
```

4. run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Relevant files

- [chat/route.ts](./app/api/chat/route.ts) handles the requests being sent to Open AI. They stream the responses back to the UI.
- [page/tsx](./app/page.tsx) handles the form, hooks and communicates with the api route.
