# TinyCPU
Design of a Simple 8-bit RISC CPU in Verilog
1. 基于有限状态机，实现了指令和状态之间的对应和转移，实现拿了取指令，指令译码，执行，访问内存和写回五个阶段的流水线。
2. 设计了8bit短指令（高三位操作码，低五位寄存器地址），16bit长指令（第一次取短指令，第二次取8bitROM或RAM地址）。
3. 指令实现了8个操作：空操作，ROM数据加载到reg，RAM数据加载到reg，reg数据写回RAM，reg数据写入累加器，累加器数据写回reg，累加器数据与reg数据相加和停机操作。
