This program is designed to disassemble given addr:instr assembly code
and print the relevant registers and values to the screen. It runs on
a linux server that contains test#.dis files in the format shown below.
It is the first program we were assigned in the introduction to
computer architecture and assembly language.

Example Output:
 
400000: j 400114
  400004: sw $ra, -4($sp)
  400008: sw $fp, -8($sp)
  
40000c: addiu $fp, $sp, -8
  400010: addiu $sp, $fp, -412
  
400014: addiu $k1, $zero, 1
  400018: sw $k1, -4($fp)
  40001c: lw $k1, -4($fp)
  
400020: addiu $k0, $zero, 100
  400024: slt $k1, $k1, $k0
  
400028: beq $k1, $zero, 4000e4
  40002c: lw $k1, 8($fp)
  400030: lui $k0, 16838
  
400034: addiu $k0, $k0, 20077
  400038: mult $k1, $k0
  40003c: mflo $k1
  
400040: addiu $k1, $k1, 12345
  400044: sw $k1, 8($fp)
  400048: lw $k1, 8($fp)
  
40004c: addiu $k0, $zero, 0
  400050: slt $k1, $k1, $k0
  
400054: beq $k1, $zero, 400068
  400058: lw $k1, 8($fp)
  40005c: lui $k0, -32768
  
400060: addu $k1, $k1, $k0
  400064: sw $k1, 8($fp)
  400068: lw $k1, 8($fp)
  
40006c: addiu $k0, $zero, 99
  400070: div $k1, $k0
  400074: mfhi $k1
  
400078: addiu $k1, $k1, 1
  40007c: sw $k1, -8($fp)
  400080: lw $k1, -4($fp)
  
400084: sll $k1, $k1, 2
  400088: addu $k1, $k1, $fp
  40008c: lw $k0, -412($k1)
  
400090: sll $k0, $k0, 3
  400094: sw $k0, -12($fp)
  400098: lw $k1, -4($fp)
  
40009c: sll $k1, $k1, 2
  4000a0: addu $k1, $k1, $fp
  4000a4: lw $k0, -8($fp)
  
4000a8: sll $k0, $k0, 2
  4000ac: addu $k0, $k0, $fp
  4000b0: lw $t9, -412($k0)
