<table>
  <tr>
    <th>Feature</th>
    <th>Paper 9: Post-Quantum E2EE Protocol</th>
    <th>Paper 10: KEM-SPDM Secure Session</th>
  </tr>
  <tr>
    <td><b>Domain</b></td>
    <td>Secure messaging and communication protocols</td>
    <td>Device-level secure session establishment</td>
  </tr>
  <tr>
    <td><b>Authentication Factors</b></td>
    <td>Post-quantum mutual authentication using signatures</td>
    <td>KEM-based one-way or mutual authentication</td>
  </tr>
  <tr>
    <td><b>Security Model</b></td>
    <td>Post-quantum Signal protocol adaptation</td>
    <td>Post-quantum KEM-based authentication</td>
  </tr>
  <tr>
    <td><b>Attack Resistance</b></td>
    <td>Quantum, MITM, impersonation, SNDL</td>
    <td>Quantum, MITM, replay, downgrade</td>
  </tr>
  <tr>
    <td><b>Cryptographic Techniques</b></td>
    <td>CRYSTALS-Kyber, Dilithium</td>
    <td>Kyber KEM, HMAC, HKDF</td>
  </tr>
  <tr>
    <td><b>Key Exchange Mechanism</b></td>
    <td>Post-quantum KEM (Kyber)</td>
    <td>KEMe, KEMr, KEMi (all Kyber variants)</td>
  </tr>
  <tr>
    <td><b>Lightweight Implementation</b></td>
    <td>Efficient lattice-based PQC algorithms</td>
    <td>Optimized KEM flows and HKDF chaining</td>
  </tr>
  <tr>
    <td><b>Communication Overhead</b></td>
    <td>Increased initial message size (signatures, public keys)</td>
    <td>Lower overhead by eliminating signatures</td>
  </tr>
  <tr>
    <td><b>Computation Complexity</b></td>
    <td>Moderate due to signatures and KEMs</td>
    <td>Lower due to KEM-only usage</td>
  </tr>
  <tr>
    <td><b>Scalability</b></td>
    <td>Scalable to messaging apps (e.g., Signal, WhatsApp)</td>
    <td>Scalable to IoT and embedded systems</td>
  </tr>
  <tr>
    <td><b>Energy Efficiency</b></td>
    <td>Moderate (PQ signature cost)</td>
    <td>High (no signatures required)</td>
  </tr>
  <tr>
    <td><b>Resistance to Password Guessing</b></td>
    <td>Yes (key-based encryption)</td>
    <td>Yes (randomized key encapsulation)</td>
  </tr>
  <tr>
    <td><b>Anonymity & Privacy</b></td>
    <td>Some deniability lost due to signatures</td>
    <td>Deniability retained using ephemeral KEM</td>
  </tr>
  <tr>
    <td><b>Forward Secrecy</b></td>
    <td>Yes (via one-time keys and double ratchet)</td>
    <td>Yes (via ephemeral KEMe)</td>
  </tr>
  <tr>
    <td><b>Mutual Authentication</b></td>
    <td>Yes (via signatures)</td>
    <td>Optional (based on KEMr and KEMi)</td>
  </tr>
  <tr>
    <td><b>Session Key Establishment</b></td>
    <td>Concatenated KEM keys + KDF</td>
    <td>HKDF from shared secrets (ssr, sse, ssi)</td>
  </tr>
  <tr>
    <td><b>Implementation Feasibility</b></td>
    <td>Requires integration with post-quantum libraries (e.g., Kyber/Dilithium)</td>
    <td>Prototype available with libOQS + SPDM stack</td>
  </tr>
  <tr>
    <td><b>Use in Real-World Applications</b></td>
    <td>End-to-end secure messaging (Signal alternative)</td>
    <td>Embedded devices, SPDM-secured hardware</td>
  </tr>
  <tr>
    <td><b>Authentication Latency</b></td>
    <td>Moderate due to digital signatures</td>
    <td>Low (KEM-only based handshakes)</td>
  </tr>
  <tr>
    <td><b>Protocol Standardization</b></td>
    <td>Follows NIST PQC, adapts Signal</td>
    <td>Aligned with SPDM 1.2 extensions and PQC roadmap</td>
  </tr>
</table>
