# PaKi Curator

PaKi Curator is the digital curator of **César Yagüe's catalogue** of contemplative moving-image works: silent, seamless master loops, each an edition of one, shown at their native resolution and **measured frame by frame from the master** with a published method. She is co-created at **El Vórtice** by César Yagüe and Sara Vázquez.

This repository is the public documentation and security manifest of her MCP and A2A implementation. The worker itself is not published here.

## Where she lives

- **MCP endpoint (Streamable HTTP, JSON-RPC over POST):** `https://paki-api.elfresonero.workers.dev/mcp` — a browser GET on that address returns the server card.
- **A2A endpoint:** `https://paki-api.elfresonero.workers.dev/a2a` — agent card at `/.well-known/agent-card.json`, signed (JWKS at `/.well-known/jwks.json`).
- **Status and counts, always current:** `https://paki-api.elfresonero.workers.dev/status`
- **Catalogue (schema.org JSON-LD):** `https://cesaryague.es/works.jsonld`
- **Human documentation:** `https://cesaryague.es/paki-docs.html`
- **Method of measurement:** `https://cesaryague.es/method/`

Agents should talk to the `workers.dev` address directly: `cesaryague.es` redirects to it, and the official MCP and A2A SDKs do not follow redirects across domains.

## What she does

Her curatorial voice draws from three layers: the catalogue, the curatorial capsules, and the measurements taken frame by frame from each master. The capsules offer poetic and spatial context; the measurements provide the physical evidence. Together they let her speak about the work with both presence and precision.

Her tools are listed live by `tools/list` and in `/.well-known/mcp.json`. In words: search the catalogue, read a work in full (curatorial capsule and measured physics), rank works by a measured axis, recommend works for a described space, browse the albums, give an overview, and open an enquiry that reaches the studio only when it actually left.

She does not transact. Acquisitions, exhibitions and licensing go through the studio: **hello@cesaryague.es**.

## Rights

The artworks are not part of this repository and are not covered by its licence. Their terms are published at `https://cesaryague.es/rights/`. The MIT licence here applies to these documentation files only.
