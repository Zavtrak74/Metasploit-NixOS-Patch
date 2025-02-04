# Metasploit-NixOS-Patch
Patch the error when running msfconsole on NixOS 24.11.714033


Full path
/nix/store/745glzbb9qzh3n9n9ylfhk7l479li1hk-metasploit-framework-6.4.35/share/msf/modules/payloads/singles/linux/riscv64le/reboot.rb
Might be different bc of the derivation


[Code]
`diff --git a/share/msf/modules/payloads/singles/linux/riscv64le/reboot.rb b/share/msf/modules/payloads/singles/linux/riscv64le/reboot.rb
deleted file mode 100644
index abcdef0..0000000
--- a/share/msf/modules/payloads/singles/linux/riscv64le/reboot.rb
+++ /dev/null
@@
-# Ce module provoque une erreur sur les architectures non-RISC-V.
-# Supprimé pour corriger l'erreur d'initialisation de la constante.
-# (Contenu original supprimé)
`
