# Rust

`merkle-tree-zk`**  
Файл: `src/main.rs`  
```rust
use ark_merkle_tree::{MerkleTree, Sha256};
let leaves = vec!["leaf1", "leaf2"];
let tree = MerkleTree::<Sha256>::new(leaves);
let proof = tree.generate_proof(0); // Доказательство для leaf1
 
