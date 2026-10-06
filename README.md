# sovern-cli ⚡

**Rent a slice of a GPU. Ship your model. Get back to the fun part.**

The official command-line tool for [SovernStack](https://sovernstack.com): fractional GPU compute, billed by the hour, built for people who train and ship models.

No dashboard. No clicking. Just your terminal and a GPU.

---

## Install

```bash
pip install sovern
```

## Quick start

Three commands from zero to a live endpoint:

```bash
# 1. Log in with your SovernStack API key
sovern login --token <your-api-key>

# 2. See what GPUs are up for grabs
sovern gpu list

# 3. Deploy your model and get a live API endpoint
sovern deploy model.onnx --name my-model
```

That's it. Go get a coffee, your endpoint will be ready before it cools down.

## What can it do?

### `sovern gpu list`

Shows which GPU capacity is available right now, so you can pick a slice that fits your workload instead of guessing.

```bash
sovern gpu list
```

### `sovern deploy`

Takes a trained model and turns it into an API endpoint.

```bash
sovern deploy model.onnx --name my-model
```

> **Heads up:** we only support **ONNX** models for now. More formats are on the way. If you've got a favorite you want to see, [open an issue](../../issues) and tell us.

## Why sovern-cli?

Because clicking through a dashboard every time you need a GPU is a vibe-killer.

SovernStack lets you rent only the VRAM you actually need (6GB, 12GB, 24GB) instead of paying for a whole card that sits there mostly idle. This CLI brings that same "take what you need, nothing more" energy to your terminal.

Built by people who got tired of watching Colab disconnect mid-training at 2am. 🫠

## Contributing

Found a bug? Got an idea? Want to add something cool? We'd love your help.

Read [CONTRIBUTING.md](CONTRIBUTING.md) to get set up, and check out issues tagged [`good first issue`](../../issues?q=label%3A%22good+first+issue%22) if you're not sure where to start.

## License

MIT. Go wild. See [LICENSE](LICENSE) for the details.
