# Rust basic REPL

1. `REPL`: `rustyline`
2. 

```rust
fn repl(env: Environment) -> Result<()> {
    loop {
        let input = rl.readline("λ => "); // rustyline
        match input {
            Ok(line) => println!("{:?}", eval(e, input)),
            _ => todo!()
        }
    }
}
```
