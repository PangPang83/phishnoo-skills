# Phishnoo Sandbox for Hermes Agent

Install this repository as a portable plugin in Hermes. Configure the operator-issued
`PHISHNOO_SANDBOX_KEY` in the active Hermes profile's secrets, then enable the plugin.
Try asking Hermes to show the sandbox P-Shield score.

The plugin ships a skill and a Streamable HTTP MCP configuration. Tool requests and
the sandbox key go to `https://api.phishnoo.nl/mcp`. The plugin marks the remote server
untrusted so Hermes asks for approval before write-capable calls. Submit synthetic
examples only. The operator supplies reviewer keys privately.

[Phishnoo](https://phishnoo.com) · [Developer docs](https://api.phishnoo.nl/docs)
