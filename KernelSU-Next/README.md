## integration

- **legacy_susfs**
```
curl -LSs "https://raw.githubusercontent.com/xxblebleblexx/KernelSU-Next/refs/heads/legacy_susfs/kernel/setup.sh" | bash -s legacy_susfs
```
- **legacy**
```
curl -LSs "https://raw.githubusercontent.com/xxblebleblexx/KernelSU-Next/refs/heads/legacy_susfs/kernel/setup.sh" | bash -s legacy
```
- **hookless**
```
curl -LSs "https://raw.githubusercontent.com/xxblebleblexx/KernelSU-Next/refs/heads/legacy_susfs/kernel/setup.sh" | bash -s hookless
```

## Instruction for legacy or legacy susfs
- patch with manual hook 

## Instruction for hookless
- Remove all manual hook implementation
- Disable ``CONFIG_KPROBES``
- Enable ``CONFIG_KSU`` and ``CONFIG_KSU_TAMPER_SYSCALL_TABLE``
- If you want add avc log spoofing enable ``CONFIG_KSU_EXTRAS``
