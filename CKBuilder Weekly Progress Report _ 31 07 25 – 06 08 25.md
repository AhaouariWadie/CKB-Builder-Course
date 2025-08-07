# Weekly Progress Report  
**Name:** Ahaouari Wadie  
**Period:** 31 July 2025 – 6 August 2025  
**Project:** Learning Nervos CKB and CCC Playground Development

---

## Summary

During this week, I focused on deepening my understanding of the Nervos CKB blockchain ecosystem, specifically the use of the CCC Playground for creating decentralized applications. My learning revolved around creating and manipulating DOBs (Digital On-Chain Objects) to model land registries, signing and verifying messages, hashing, and building basic transfer functions. I also explored transaction construction, cell management, and best practices for creating a simple land registry DApp. This foundational work prepares me for developing more complex DApps, such as token issuance and NFT-based land registries.

---

## Detailed Daily Activities

### Monday, 31 July 2025  
- Introduced to the CCC Playground environment and connected wallet (JoyID).  
- Explored basic concepts: signers, transactions, and how to sign and verify messages on the playground.  
- Practiced signing a message and verifying its signature using the CCC connector.

### Tuesday, 1 August 2025  
- Studied hashing functions available in CCC (hashCkb with UTF-8 and hex inputs).  
- Learned how to convert strings to bytes and hash them properly.  
- Experimented with signing and verifying using React components in the playground environment.

### Wednesday, 2 August 2025  
- Deep-dived into transaction building basics on Nervos CKB using CCC SDK.  
- Practiced constructing transactions with outputs and outputsData, completing inputs, and paying transaction fees.  
- Learned how to retrieve the recommended address from the signer.

### Thursday, 3 August 2025  
- Developed a simple transfer DApp that creates transactions sending CKB to a single address.  
- Implemented UI components with React for inputting addresses, amounts, and optional output data.  
- Learned about transaction completion helpers like `completeInputsByCapacity` and `completeFeeBy`.

### Friday, 4 August 2025  
- Explored the concept of DOBs (Digital On-Chain Objects) as immutable land registry records.  
- Wrote a script to issue multiple land parcels as DOBs on the blockchain to build a simple land registry.  
- Understood the importance of immutability and data stored in outputsData of cells.

### Saturday, 5 August 2025  
- Designed and prototyped a subdivision approach for land parcels using DOBs in CCC Playground.  
- Learned to consume an original DOB and create multiple new DOBs in the same transaction to simulate parcel splitting.  
- Practiced handling transaction inputs, outputs, and outputsData for subdivision.

### Sunday, 6 August 2025  
- Planned next steps for building a complete land registry DApp, including indexing DOBs, building a React UI for display and parcel registration.  
- Reviewed architectural choices between subdivision and fractionalization approaches for land ownership.  
- Outlined possible extensions such as ownership transfer, validation, and dispute resolution.

---

## Goals for Next Week (7 August – 13 August 2025)

- Build a React-based UI for reading and displaying land parcel DOBs from the Nervos CKB blockchain.  
- Integrate wallet connection and live data querying via CKB Indexer or JSON-RPC APIs.  
- Implement a parcel registration form that creates new DOBs on the blockchain.  
- Add basic search and filtering capabilities by parcel attributes (plot number, owner name).  
- Explore transaction signing and sending flows in the UI for enhanced user experience.

---

*Prepared by Ahaouari Wadie*  
*Date: 6 August 2025*
