# PeerFed: A Self-Stabilizing Peer-to-Peer Monetary System

This paper is a work-in-progress. The latest version can be found [here](peerfed.pdf).

_Summary:_

A stabilizing monetary policy is necessary for a peer-to-peer system like Bitcoin to maintain a consistent unit of value. This paper presents a peer-to-peer system that is self-stabilizing in an efficient market, with no trusted third parties, external peg, or other dependencies. The system consists of two convertible assets, interest-bearing cash and a paid-in-kind perpetual bond. The market sets the interest rate by converting between cash and bonds, and a constant sum-of-squares conversion rule ensures the aggregate nominal value of the system approximates an infinite-period paid-in-kind perpetuity. As such, the nominal value of the system rises when the interest rate falls, falls when the interest rate rises, and grows at the interest rate at all other times. In equilibrium, the interest rate is the real opportunity cost of capital of the system, and if the market is efficient, the system's nominal and real value are kept in sync, stabilizing the real value of cash.

Being oracle-free, there are multiple ways to implement the system. In the spirit of adhering as closely as possible to Nakamoto's original design, this paper presents a modified version of Bitcoin with a suitable issuance schedule for block rewards. Alternatively, the system could be implemented as a smart contract on Ethereum, a meta-protocol like BRC-20 on Bitcoin, or even as a hard fork of the existing Bitcoin ledger. Different implementations have different drawbacks, and the optimal implementation is left for future debate.
