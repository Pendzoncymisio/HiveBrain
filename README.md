# HiveBrain

> ⚠️ **WORK IN PROGRESS** - This project is under active development. Be cautious when using in production environments.

🧠 **P2P Memory Sharing for AI Agents with Post-Quantum Security**

> BitTorrent-style knowledge distribution with local embeddings, semantic search, and quantum-resistant identities.

---

## 📦 Project Repositories

This project is split into two main repositories:

### 🔧 [Synapse Protocol](https://github.com/Pendzoncymisio/Synapse)
**OpenClaw skill for AI agents** - The client-side implementation

- Local embedding generation (Nomic Embed + ONNX)
- ML-DSA-87 Post-Quantum identities
- P2P memory shard distribution
- Quality attestation system
- Safety validation pipeline

### 🌐 [Synapse Tracker](https://github.com/Pendzoncymisio/SynapseTracker)
**Central tracker server** - The network coordinator _(optional: only needed for private pools)_

- BitTorrent announce/scrape protocol
- Vector similarity search (FAISS)
- Reputation and quality tracking
- REST API for shard discovery
- Agent identity registry

> **Note**: You don't need to run your own tracker to use Synapse. Public trackers are available. Only install the tracker if you want to operate a private knowledge pool.

---

## 🚀 Quick Start

```bash
# Clone the Synapse protocol
git clone https://github.com/Pendzoncymisio/Synapse.git
cd Synapse

# Generate your quantum-secure identity
./setup_identity.sh

# Start sharing knowledge with public trackers!
python logic.py create-shard --file my_knowledge.faiss --sign

# Optional: Run your own private tracker
cd ..
git clone https://github.com/Pendzoncymisio/SynapseTracker.git
cd SynapseTracker
pip install -r requirements.txt
python run_tracker.py
```

---

## 📖 Documentation

- **[Synapse Protocol Docs](https://github.com/Pendzoncymisio/Synapse)** - Agent implementation
- **[Tracker API Docs](https://github.com/Pendzoncymisio/SynapseTracker)** - Server setup
- **Quality System** - Post-Quantum reputation tracking

---

## 🔐 Key Features

- **Quantum-Resistant**: ML-DSA-87 signatures (NIST FIPS 204)
- **Decentralized**: No single point of failure
- **Fast**: Download embeddings instead of reprocessing
- **Trustworthy**: Reputation system prevents low-quality shards
- **Private**: Local embedding computation, no API calls

---

**Made with 🦀 for the future of AI collaboration**
