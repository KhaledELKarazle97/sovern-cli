# sovernslice

The official command-line tool for [SovernStack](https://sovernstack.com) — fractional GPU compute, billed by the hour, built for AI researchers and developers.

List available GPUs, deploy your trained models, and manage your compute without leaving the terminal.

## Install

```bash
pip install sovernslice
```

## Quick start

```bash
# Authenticate with your SovernStack API key
sovernslice login --token <your-api-key>

# See what GPU capacity is available
sovernslice gpu list

# Deploy a trained model and get a live API endpoint
sovernslice deploy model.onnx --name my-model
```

## Why sovernslice?

SovernStack lets you rent only the GPU memory you actually need, 6GB, 12GB, or 24GB, instead of paying for a whole card you won't fully use. This CLI brings that same philosophy to your terminal: fast, scriptable, and built for people who'd rather not click through a dashboard every time.

## Contributing

This project is open source and we'd love your help. Check out [CONTRIBUTING.md](CONTRIBUTING.md) to get started, and look for issues tagged [`good first issue`](../../issues?q=label%3A%22good+first+issue%22) if you're not sure where to begin.

## License

MIT — see [LICENSE](LICENSE) for details.
