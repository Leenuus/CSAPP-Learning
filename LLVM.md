## LLVM

LLVM(low level virtual machine), a compiler building framework invented in 2003. LLVM stands for this project, also the tools it distributes, such as `clang`, `opt`, `lldb`(debugger), `lld`(linker)

### Architecture

Front end: From language-dependant code to IR, Intermediate Code in LLVM; for example, `rustc`

Middle end: executable `opt`, it can generate optimized code from IR to IR. IR is in ascii, not in binary. `opt` can generate **graph representation** of the code too.

Back end: Generate __platform-dependant__ code from IR to IR, then the IR can be compile into binary with platform tools like `as` on Linux
