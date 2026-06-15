# Event-SImulator-JS
## 🎪 Festival Gate Simulation

Ever wondered what happens when too many people show up to a festival at once? This little JS simulation models exactly that — attendees flowing through entry gates, gates hitting capacity, and overflow crowds getting rerouted to keep things moving.

## ⚙️ How it works

Picture four gates — **North, East, South, West** — each with its own processing capacity and a queue of attendees arriving over time.

- ⏱️ The simulation runs in **ticks** (think of each tick as a time slot, like every 15 minutes).
- 🚪 At each tick, every gate processes as many attendees as its `capacity` allows.
- 🌊 If a gate can't keep up and people are left waiting, that **overflow** gets rerouted to the *next* gate in line — round-robin style.
- 📊 At the end, a summary tallies up exactly how many attendees each gate processed in total.

## 🌅 🌙 Two scenarios

The simulation runs twice:
- **Morning** — a different mix of crowd sizes and gate capacities
- **Night** — busier gates, different bottlenecks

Watch the console output to see crowds shift between gates in real time as overflow gets handled.

## ▶️ Running it

```bash
node festival.js
```

You'll see a tick-by-tick breakdown of arrivals, processing, and any rerouting — followed by a final throughput summary for each gate.

## 🧠 Concepts practiced

`for` / `while` loops, object & array manipulation, modular functions, modulo-based wraparound logic, and accumulator patterns.
