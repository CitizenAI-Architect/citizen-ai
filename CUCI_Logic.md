# CUCI Logic: The Vault & Hybrid Anchor (Final Spec)

## 1. The Fog Engine (Under the Hood)
The mathematical algorithm responsible for data fragmentation and encryption.
- **Operation:** Works invisibly "under the hood" to ensure a seamless experience.
- **Personalized Fog:** Generates a unique "Mathematical Salt" (Personal Seed) during first activation, ensuring unique fog signatures for every user.
- **Block-Level Processing (Chunking):** The Vault is divided into small encrypted blocks. This prevents sync conflicts and allows updating only changed parts of the data.

## 2. The Vault Protocol (Safe-within-a-Safe)
- **Storage:** The cloud provider sees only an obfuscated collection of binary blocks.
- **Visibility:** Internal structures (filenames, hierarchy, metadata) are completely hidden.
- **Data Padding:** The system adds "noise" to blocks to mask the actual size and type of the files.
- **RAM-Only Processing:** Decryption occurs strictly in the device's volatile memory (RAM) to prevent data leaks to the physical drive.

## 3. The Hybrid Key (The Lens Trigger)
- **Static Part (The "Dead" Key):** An encrypted file-based backup containing the "Personal Seed". It is useless without the activation pulse.
- **Dynamic Part (The "Live" Impulse):**
    - **Fast Access:** Biometric activation for daily local use on trusted devices.
    - **Sovereign Access:** A passphrase or numerical code stored only in the user's mind.
    - **Panic Code (Optional):** A secondary code that triggers a decoy environment (empty vault).

## 4. Visual Sovereign Status (The Vault UI)
- **Status Metamorphosis:** Upon activation, the standard cloud provider icon is replaced by the "Sovereign Vault" icon.
- **Deletion Protection:** The Vault object is locked at the OS level. Removal or uninstallation requires the "Sovereign Access" code to prevent accidental or unauthorized data loss.

## 5. Metadata & Traffic Protection
- **Zero-Knowledge:** No passphrase storage. The system never "knows" your secret.
- **Activity Masking:** Masks file count, exact sizes, and update frequencies from the cloud provider, making user activity indistinguishable from random noise.

## 6. Recovery & Resilience
- **Reconstruction:** Combining the Static Backup with the Sovereign Access code re-mounts the Vault on any clean device.
- **Persistence:** The protocol ensures that as long as the user remembers the Sovereign Access code and has access to the "Dead Key" (from any source), their digital identity and data are indestructible.
