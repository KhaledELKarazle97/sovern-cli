# sovern-cli

The official command-line tool for [SovernStack](https://sovernstack.com) - fractional GPU compute, billed by the hour, built for AI researchers and developers.

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

## Why sovern-cli?

Because clicking through a dashboard every time you need a GPU is a vibe-killer.

SovernStack lets you rent only the VRAM you actually need, 6GB, 12GB, 24GB, instead of paying for a whole card to sit there mostly idle. This CLI brings that same "take what you need, nothing more" energy to your terminal. List GPUs, ship your model, get an endpoint. No dashboard, no clicking, no waiting around.

Built by people who got tired of watching Colab disconnect mid-training at 2am.

## Contributing

This project is open source and we'd love your help. Check out [CONTRIBUTING.md](CONTRIBUTING.md) to get started, and look for issues tagged [`good first issue`](../../issues?q=label%3A%22good+first+issue%22) if you're not sure where to begin.

## License

MIT — see [LICENSE](LICENSE) for details.
