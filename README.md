# CareFlow Patient Queue

A demo hospital patient queue dashboard based on the supplied Hospital Patient Queue System brief.

## Run in Replit

Open the project and run the `artifacts/patient-queue: web` workflow.

## Run from a local shell

Requires Node.js 24 and pnpm. From the project root:

```sh
pnpm install
PORT=5173 BASE_PATH=/ pnpm --filter @workspace/patient-queue run dev
```

Open the local URL printed by Vite. Patient records are demo data stored in browser localStorage; do not enter real patient or clinical information. Wait estimates are illustrative and are not clinical guidance.

The queue sorts by triage priority ascending (1 is highest urgency), then by arrival order for patients sharing a priority. The Heap Inspector demonstrates this ordering in the browser; it is a visual demonstration, not a C++ runtime.
