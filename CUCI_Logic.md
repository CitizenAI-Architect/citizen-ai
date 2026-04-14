# CUCI Logic: The Vault & Hybrid Anchor

## 1. The Fog Engine (Under the Hood)
The mathematical algorithm responsible for data fragmentation and encryption.
- **Operation:** Works invisibly to ensure a seamless "plug-and-play" experience.
- **Personalized Fog:** During first activation, the engine generates a unique "Mathematical Salt" (Personal Seed). This ensures that even with the same code, every user produces a unique "fog signature".

## 2. The Vault Protocol (Safe-within-a-Safe)
Instead of encrypting individual files, the system creates an obfuscated virtual container (The Vault).
- **Storage:** The cloud provider sees only one large, encrypted binary object.
- **Visibility:** Internal structures (filenames, hierarchy, metadata) are completely hidden.
- **Scalability:** The Vault is designed to match the user's cloud storage capacity (e.g., if the cloud is 1TB, the Vault operates within that 1TB).

## 3. The Hybrid Key (The Lens Trigger)
The mechanism that activates the Fog Engine to "unfog" the Vault. It consists of two parts:

- **Static Part (The "Dead" Key):** An encrypted file-based backup containing the "Personal Seed". It can be stored anywhere as it remains useless without the activation pulse.
- **Dynamic Part (The "Live" Impulse):**
    - **Fast Access:** Biometric activation for daily local use on trusted devices.
    - **Sovereign Access:** A passphrase or numerical code stored only in the user's mind. Essential for recovery on new devices and "resurrecting" the Dead Key.

## 4. Security & Hardening
- **Zero-Knowledge:** The system never stores the user's passphrase.
- **Collision Resistance:** Personal Seeds prevent different users' data from overlapping.
- **Metadata Protection:** The Vault structure prevents the cloud provider from analyzing file types, sizes, or update frequencies.

## 5. Recovery Protocol
Recovery is performed by combining the Static Backup (Dead Key) from any source with the Sovereign Access code provided by the user. This re-mounts the Vault on any clean device.
